# LearnPython


1.QDialog，直接有exec_()方法来设置模态对话框，QWidget没有。

  
2.QSize怎么才能直接用呢？
  现状是 
  from PyQt5 import QtCore
  
  self.dlg.setMinimumSize(QtCore.QSize(700,700))
  
3. Qt.ApplicationModal怎么才能直接用
 
  self.dlg.setWindowModality(2) #ApplicationModal)
  
  可以这样用
  
  from PyQt5.QtCore import Qt

  self.dlg.setWindowModality(Qt.ApplicationModal)
