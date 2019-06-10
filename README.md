# LearnPython


1.QDialog，直接有exec_()方法来设置模态对话框，QWidget没有。

  
2.QSize怎么才能直接用呢？
  现状是 
  from PyQt5 import QtCore
  
  self.dlg.setMinimumSize(QtCore.QSize(700,700))
  
  
  可以这样:
  from PyQt5.QtCore import QSize
  self.dlg.setMinimumSize(QSize(700,700))
  
3. Qt.ApplicationModal怎么才能直接用
 
  self.dlg.setWindowModality(2) #ApplicationModal)
  
  可以这样用
  
  from PyQt5.QtCore import Qt

  self.dlg.setWindowModality(Qt.ApplicationModal)
  
  
  
 4.各种数据格式的转换
  浮点数转字节（小端，大端）
  整数转字节（小端，大端）
  字符串转字节
  16进制字符串转字节
  字节转字符串
  （“0xef9078”）
  
  
 
