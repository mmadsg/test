from asyncio.windows_events import NULL
from pandas.plotting import table 
from cmath import nan
from fileinput import close
import os
from pickle import TRUE
from time import time
from tkinter import END
from tkinter.tix import COLUMN
#from types import NoneType
from unicodedata import name
import MetaTrader5 as mt5
import datetime
import yfinance as yf
from pandas_datareader import data as pdr
import pandas as pd
import numpy as np
from pandas.plotting import register_matplotlib_converters
from colorama import Fore
import talib
import threading
from pandas.plotting import table
from matplotlib.pyplot import figure as fig
import dataframe_image as dfi
from PIL import Image, ImageFile
import os
import smtplib
from email.mime.text import MIMEText
from email.mime.image import MIMEImage
from email.mime.multipart import MIMEMultipart
import pywhatkit
import sys
from PyQt5 import *
from PyQt5.QtCore import *
from PyQt5.QtGui import *
from PyQt5.QtWidgets import *
import psutil


class Ui_MainWindow(object):
        emaills=None
        excells=True
        whatsss=None
        piccs=True
        numbers='+989215723787'
        timefr='10m'
        timefrTR='60m'
        emailadres=None
        dayss='10d'
        dayskala = 3
        nam=[]
        thread = 3600

        
        def setupUi(self, MainWindow):
                
             #if MainWindow.objectName():
                MainWindow.setObjectName("MainWindow")
                MainWindow.resize(1101, 820)
                MainWindow.setStyleSheet("background-color: rgb(0, 0, 0);")
                self.centralwidget = QWidget(MainWindow)
                self.centralwidget.setObjectName("centralwidget")
                self.label_3 = QLabel(self.centralwidget)
                self.label_3.setObjectName("label_3")
                self.label_3.setGeometry(QRect(320, 480, 71, 21))
                self.label_3.setStyleSheet("color: rgb(255, 255, 255);")
                self.DAYSNUMBER = QLCDNumber(self.centralwidget)
                self.DAYSNUMBER.setObjectName("DAYSNUMBER")
                self.DAYSNUMBER.setGeometry(QRect(338, 405, 101, 81))
                self.DAYSNUMBER.setProperty("value", 3)
                self.symbols = QPlainTextEdit(self.centralwidget)
                self.symbols.setObjectName("symbols")
                self.symbols.setGeometry(QRect(0, 130, 391, 101))
                self.symbols.setStyleSheet("color: rgb(255, 255, 255);\n"
        "background-color: rgb(85, 0, 0);")
                self.symbols.setOverwriteMode(True)
                self.TIMEFRAME = QLCDNumber(self.centralwidget)
                self.TIMEFRAME.setObjectName("TIMEFRAME")
                self.TIMEFRAME.setGeometry(QRect(328, 285, 101, 81))
                self.TIMEFRAME.setStyleSheet("")
                self.TIMEFRAME.setProperty("value", 10.000000000000000)

                self.symbols.setOverwriteMode(True)
                self.INTERVAL_Trendlcd = QLCDNumber(self.centralwidget)
                self.INTERVAL_Trendlcd.setObjectName("Interval_Trend")
                self.INTERVAL_Trendlcd.setGeometry(QRect(338, 520, 101, 81))
                self.INTERVAL_Trendlcd.setStyleSheet("")
                self.INTERVAL_Trendlcd.setProperty("value", 60.000000000000000)

                self.label_10 = QLabel(self.centralwidget)
                self.label_10.setObjectName("label_10")
                self.label_10.setGeometry(QRect(310, 580, 171, 20))
                self.label_10.setStyleSheet("color: rgb(255, 255, 255);")

                self.label_2 = QLabel(self.centralwidget)
                self.label_2.setObjectName("label_2")
                self.label_2.setGeometry(QRect(320, 360, 171, 20))
                self.label_2.setStyleSheet("color: rgb(255, 255, 255);")
                self.giveme = QPushButton(self.centralwidget)
                self.giveme.setObjectName("giveme")
                self.giveme.setGeometry(QRect(260, 660, 611, 111))
                self.giveme.setStyleSheet("background-color: rgb(255, 181, 32);")
                self.OUTPUTOPTIONS = QFrame(self.centralwidget)
                self.OUTPUTOPTIONS.setObjectName("OUTPUTOPTIONS")
                self.OUTPUTOPTIONS.setGeometry(QRect(630, 170, 461, 351))
                self.OUTPUTOPTIONS.setStyleSheet("background-color: rgb(255, 121, 123);\n"
        "background-color: rgb(255, 253, 228);")
                self.OUTPUTOPTIONS.setFrameShape(QFrame.StyledPanel)
                self.OUTPUTOPTIONS.setFrameShadow(QFrame.Raised)
                self.pic = QCheckBox(self.OUTPUTOPTIONS)
                self.pic.setObjectName("pic")
                self.pic.setGeometry(QRect(10, 0, 161, 61))
                self.pic.setStyleSheet("font: 11pt \"MS Shell Dlg 2\";")
                self.pic.setChecked(True)
                self.whats = QCheckBox(self.OUTPUTOPTIONS)
                self.whats.setObjectName("whats")
                self.whats.setGeometry(QRect(10, 90, 111, 71))
                self.whats.setStyleSheet("font: 11pt \"MS Shell Dlg 2\";")
                self.whats.setChecked(False)
                self.excel = QCheckBox(self.OUTPUTOPTIONS)
                self.excel.setObjectName("excel")
                self.excel.setGeometry(QRect(10, 180, 111, 81))
                self.excel.setStyleSheet("font: 11pt \"MS Shell Dlg 2\";")
                self.excel.setChecked(True)
                self.email = QCheckBox(self.OUTPUTOPTIONS)
                self.email.setObjectName("email")
                self.email.setGeometry(QRect(10, 270, 101, 61))
                self.email.setStyleSheet("font: 11pt \"MS Shell Dlg 2\";")
                self.emailadress = QPlainTextEdit(self.OUTPUTOPTIONS)
                self.emailadress.setObjectName("emailadress")
                self.emailadress.setEnabled(False)
                self.emailadress.setGeometry(QRect(150, 290, 271, 31))
                self.emailadress.setFocusPolicy(Qt.ClickFocus)
                self.emailadress.setAcceptDrops(False)
                self.emailadress.setStyleSheet("background-color: rgb(161, 161, 161);")
                self.emailadress.setInputMethodHints(Qt.ImhEmailCharactersOnly|Qt.ImhLatinOnly)
                self.emailadress.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
                self.emailadress.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
                self.emailadress.setSizeAdjustPolicy(QAbstractScrollArea.AdjustToContents)
                self.emailadress.setTabChangesFocus(True)
                self.emailadress.setLineWrapMode(QPlainTextEdit.WidgetWidth)
                self.emailadress.setOverwriteMode(False)
                self.phonenumber = QPlainTextEdit(self.OUTPUTOPTIONS)
                self.phonenumber.setObjectName("phonenumber")
                self.phonenumber.setEnabled(True)
                self.phonenumber.setGeometry(QRect(150, 110, 271, 31))
                self.phonenumber.setFocusPolicy(Qt.ClickFocus)
                self.phonenumber.setAcceptDrops(False)
                self.phonenumber.setStyleSheet("background-color: rgb(161, 161, 161);")
                self.phonenumber.setInputMethodHints(Qt.ImhLatinOnly)
                self.phonenumber.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
                self.phonenumber.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
                self.phonenumber.setSizeAdjustPolicy(QAbstractScrollArea.AdjustToContents)
                self.phonenumber.setTabChangesFocus(True)
                self.phonenumber.setReadOnly(False)
                self.phonenumber.setOverwriteMode(False)
                self.phonenumber.setTextInteractionFlags(Qt.TextEditorInteraction)
                self.label_5 = QLabel(self.OUTPUTOPTIONS)
                self.label_5.setObjectName("label_5")
                self.label_5.setGeometry(QRect(240, 90, 101, 16))
                self.label_6 = QLabel(self.OUTPUTOPTIONS)
                self.label_6.setObjectName("label_6")
                self.label_6.setGeometry(QRect(230, 270, 101, 16))
                self.days = QScrollBar(self.centralwidget)
                self.days.setObjectName("days")
                self.days.setGeometry(QRect(0, 420, 381, 51))
                self.days.setStyleSheet("background-color: rgb(148, 223, 255);")
                self.days.setMaximum(1000)
                self.days.setSingleStep(1)
                self.days.setPageStep(100)
                self.days.setValue(3)
                self.days.setOrientation(Qt.Horizontal)
                self.exit = QPushButton(self.centralwidget)
                self.exit.setObjectName("exit")
                self.exit.setGeometry(QRect(0, 720, 101, 51))
                self.exit.setStyleSheet("color: rgb(175, 0, 0);\n"
        "background-color: rgb(255, 250, 230);")
                self.INTERVAL = QScrollBar(self.centralwidget)
                self.INTERVAL.setObjectName("INTERVAL")
                self.INTERVAL.setGeometry(QRect(0, 300, 381, 51))
                self.INTERVAL.setStyleSheet("background-color: rgb(93, 203, 137);")
                self.INTERVAL.setMinimum(1)
                self.INTERVAL.setMaximum(1000)
                self.INTERVAL.setSingleStep(1)
                self.INTERVAL.setValue(10)
                self.INTERVAL.setOrientation(Qt.Horizontal)

                self.INTERVAL_Trend = QScrollBar(self.centralwidget)
                self.INTERVAL_Trend.setObjectName("INTERVAL_Trend")
                self.INTERVAL_Trend.setGeometry(QRect(0, 530, 381, 51))
                self.INTERVAL_Trend.setStyleSheet("background-color: rgb(93, 203, 137);")
                self.INTERVAL_Trend.setMinimum(1)
                self.INTERVAL_Trend.setMaximum(1000)
                self.INTERVAL_Trend.setSingleStep(1)
                self.INTERVAL_Trend.setValue(60)
                self.INTERVAL_Trend.setOrientation(Qt.Horizontal)

                self.textBrowser = QTextBrowser(self.centralwidget)
                self.textBrowser.setObjectName("textBrowser")
                self.textBrowser.setGeometry(QRect(910, 0, 181, 31))
                self.label = QLabel(self.centralwidget)
                self.label.setObjectName("label")
                self.label.setGeometry(QRect(140, 105, 111, 21))
                self.label.setStyleSheet("color: rgb(255, 255, 255);\n"
        "font: 14pt \"Times New Roman\";")
                self.label_4 = QLabel(self.centralwidget)
                self.label_4.setObjectName("label_4")
                self.label_4.setGeometry(QRect(720, 140, 281, 31))
                self.label_4.setStyleSheet("color: rgb(255, 255, 255);\n"
        "font: 18pt \"Times New Roman\";")
                self.label_9 = QLabel(self.centralwidget)
                self.label_9.setObjectName("label_4")
                self.label_9.setGeometry(QRect(0, 250, 350, 41))
                self.label_9.setStyleSheet("color: rgb(255, 255, 255);\n"
        "font: 10pt \"Times New Roman\";")
                MainWindow.setCentralWidget(self.centralwidget)
                self.menubar = QMenuBar(MainWindow)
                self.menubar.setObjectName("menubar")
                self.menubar.setGeometry(QRect(0, 0, 1101, 26))
                MainWindow.setMenuBar(self.menubar)
                self.statusbar = QStatusBar(MainWindow)
                self.statusbar.setObjectName("statusbar")
                MainWindow.setStatusBar(self.statusbar)

                self.retranslateUi(MainWindow)
                
                self.whats.toggled.connect(self.whatss)

                self.phonenumber.textChanged.connect(self.number)

                self.email.toggled.connect(self.emailadress.setEnabled)
                self.email.toggled.connect(self.emailadress.clear)
                self.email.toggled.connect(self.emaill)

                self.emailadress.textChanged.connect(self.mailing)
                
                self.pic.toggled.connect(self.picc)
                
                self.excel.toggled.connect(self.excell)
                
                self.days.valueChanged.connect(self.DAYSNUMBER.display)
                self.INTERVAL.valueChanged.connect(self.TIMEFRAME.display)
                self.INTERVAL_Trend.valueChanged.connect(self.INTERVAL_Trendlcd.display)
                self.INTERVAL.valueChanged.connect(self.timfrfun)
                self.INTERVAL_Trend.valueChanged.connect(self.timfrfun)
                self.DAYSNUMBER.overflow.connect(self.daynum)
                self.symbols.textChanged.connect(self.sym)
                self.exit.clicked.connect(MainWindow.close)
                self.giveme.clicked.connect(self.body)

                QMetaObject.connectSlotsByName(MainWindow)
        # setupUi
        def sym(self):
         
         matnn = self.symbols.toPlainText()
         matn = self.symbols.toPlainText().splitlines()
        
         if matnn.endswith('\n'):
                self.nam.clear()
                for line in matn:
                
                 self.nam.append(line)
                
         self.nam = list(filter(None, self.nam))
        
        def mailing(self):

         self.emailadres = self.emailadress.toPlainText()
        
        def daynum(self):
        
         
         self.dayss = str(self.DAYSNUMBER.value()+'d')

        def timfrfun(self):
         
         self.thread = 60*self.INTERVAL.value()
         self.timefr = str(self.INTERVAL.value())+'m'
         self.timefrTR = str(self.INTERVAL_Trend.value())+'m'
         self.out = self.time_frame_converter()

        def number(self):
         self.numbers = str('+'+self.phonenumber.toPlainText())
         
        def picc(self):
         
         if self.piccs == True:
            self.piccs = False
         else: self.piccs = True

        def whatss(self):
         if self.whatsss == True:
            self.whatsss = False
         else: self.whatsss = True

        def excell(self):
         
         if self.excells == True:
            self.excells = False
         else: self.excells = True
        
        def emaill(self):
         
         if self.excells == True:
            self.emaills = False
         else: self.emaills = True

        def SendMail(self,ImgFileName):
                with open(ImgFileName, 'rb') as f:
                        img_data = f.read()
                msg = MIMEMultipart()
                msg['Subject'] = 'خروجی نرم‌افزار'
                #msg['From'] = 'farevahar_4444@yahoo.com'
                msg['To'] = self.emailadres

                text = MIMEText(ImgFileName)
                msg.attach(text)
                image = MIMEImage(img_data, name=os.path.basename(ImgFileName))
                msg.attach(image)

                s = smtplib.SMTP('smtp.mail.yahoo.com',587)
                s.ehlo()
                s.starttls()
                s.ehlo()
                s.login('farevahar_4444@yahoo.com', 'adqljyvysupskkwp')
                s.sendmail('farevahar_4444@yahoo.com', str(self.emailadres), msg.as_string())
                s.quit()

        def body(self):
                #wb = xl.Workbook()
                #wb.save(r"C:\Users\Mmad\Desktop\KHOROJI PYTHON\RESULT.xlsx")
                tm=60*self.INTERVAL.value()
                ##print(tm)
                threading.Timer(tm, self.body).start()
              #  if len(self.nam) != 0:
               #         for j in range(len(self.nam)):
                for proc in psutil.process_iter():
                        if proc.name() == "Microsoft.Photos.exe":
                            proc.kill()
                for sy in self.nam:
                        ##print('\n\n',sy,'\n\n' )
                        self.calculation(sy,self.calculation_TREND(sy))
                
        def time_frame_converter(self):
            if self.INTERVAL.value() == 800: return(mt5.TIMEFRAME_D1)
            elif self.INTERVAL.value() == 900: return(mt5.TIMEFRAME_W1)
            elif self.INTERVAL.value() == 1000: return(mt5.TIMEFRAME_MN1)
            elif self.INTERVAL.value() == 30: return(mt5.TIMEFRAME_M30)
            elif self.INTERVAL.value() == 120: return(mt5.TIMEFRAME_H2)
            elif self.INTERVAL.value() == 180: return(mt5.TIMEFRAME_H3)
            elif self.INTERVAL.value() == 240: return(mt5.TIMEFRAME_H4)
            elif self.INTERVAL.value() == 360: return(mt5.TIMEFRAME_H6)
            elif self.INTERVAL.value() == 480: return(mt5.TIMEFRAME_H8)
            elif self.INTERVAL.value() == 720: return(mt5.TIMEFRAME_H12)
            elif self.INTERVAL.value() == 1: return(mt5.TIMEFRAME_M1)
            elif self.INTERVAL.value() == 2: return(mt5.TIMEFRAME_M2)
            elif self.INTERVAL.value() == 3: return(mt5.TIMEFRAME_M3)
            elif self.INTERVAL.value() == 4: return(mt5.TIMEFRAME_M4)
            elif self.INTERVAL.value() == 6: return(mt5.TIMEFRAME_M6)
            elif self.INTERVAL.value() == 10: return(mt5.TIMEFRAME_M10)
            elif self.INTERVAL.value() == 12: return(mt5.TIMEFRAME_M12)
            elif self.INTERVAL.value() == 15: return(mt5.TIMEFRAME_M15)
            elif self.INTERVAL.value() == 20: return(mt5.TIMEFRAME_M20)
            else: return(mt5.TIMEFRAME_H1)

        def time_frame_converter_TR(self):
            if self.INTERVAL_Trend.value() == 800: return(mt5.TIMEFRAME_D1)
            elif self.INTERVAL_Trend.value() == 900: return(mt5.TIMEFRAME_W1)
            elif self.INTERVAL_Trend.value() == 1000: return(mt5.TIMEFRAME_MN1)
            elif self.INTERVAL_Trend.value() == 30: return(mt5.TIMEFRAME_M30)
            elif self.INTERVAL_Trend.value() == 120: return(mt5.TIMEFRAME_H2)
            elif self.INTERVAL_Trend.value() == 180: return(mt5.TIMEFRAME_H3)
            elif self.INTERVAL_Trend.value() == 240: return(mt5.TIMEFRAME_H4)
            elif self.INTERVAL_Trend.value() == 360: return(mt5.TIMEFRAME_H6)
            elif self.INTERVAL_Trend.value() == 480: return(mt5.TIMEFRAME_H8)
            elif self.INTERVAL_Trend.value() == 720: return(mt5.TIMEFRAME_H12)
            elif self.INTERVAL_Trend.value() == 1: return(mt5.TIMEFRAME_M1)
            elif self.INTERVAL_Trend.value() == 2: return(mt5.TIMEFRAME_M2)
            elif self.INTERVAL_Trend.value() == 3: return(mt5.TIMEFRAME_M3)
            elif self.INTERVAL_Trend.value() == 4: return(mt5.TIMEFRAME_M4)
            elif self.INTERVAL_Trend.value() == 6: return(mt5.TIMEFRAME_M6)
            elif self.INTERVAL_Trend.value() == 10: return(mt5.TIMEFRAME_M10)
            elif self.INTERVAL_Trend.value() == 12: return(mt5.TIMEFRAME_M12)
            elif self.INTERVAL_Trend.value() == 15: return(mt5.TIMEFRAME_M15)
            elif self.INTERVAL_Trend.value() == 20: return(mt5.TIMEFRAME_M20)
            else: return(mt5.TIMEFRAME_H1)
        
        def retranslateUi(self, MainWindow):
                MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", "MainWindow", None))
                self.label_3.setText(QCoreApplication.translate("MainWindow", "DAYS", None))
                self.symbols.setPlainText(QCoreApplication.translate("MainWindow", u"\n" 
        , None))
                self.label_2.setText(QCoreApplication.translate("MainWindow", "INTERVAL IN MINUTES", None))
                self.label_10.setText(QCoreApplication.translate("MainWindow", "Trend Interval", None))
                self.giveme.setText(QCoreApplication.translate("MainWindow", "GIVE ME AN OUTPUT", None))
                self.pic.setText(QCoreApplication.translate("MainWindow", "SHOW PICTURES", None))
                self.whats.setText(QCoreApplication.translate("MainWindow", "WHATSAPP", None))
                self.excel.setText(QCoreApplication.translate("MainWindow", "EXCELLS", None))
                self.email.setText(QCoreApplication.translate("MainWindow", "EMAIL", None))
                self.emailadress.setPlainText(QCoreApplication.translate("MainWindow", " @gmail.com", None))
                self.phonenumber.setPlainText(QCoreApplication.translate("MainWindow", "989215723787", None))
                self.label_5.setText(QCoreApplication.translate("MainWindow", "PHONE NUMBER", None))
                self.label_6.setText(QCoreApplication.translate("MainWindow", "EMAIL ADDRESS", None))
                self.exit.setText(QCoreApplication.translate("MainWindow", "BYE-BYE", None))
                self.textBrowser.setHtml(QCoreApplication.translate("MainWindow", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
        "<html><head><meta name=\"qrichtext\" content=\"1\" /><style type=\"text/css\">\n"
        "p, li { white-space: pre-wrap; }\n"
        "</style></head><body style=\" font-family:'MS Shell Dlg 2'; font-size:7.8pt; font-weight:400; font-style:normal;\">\n"
        "<p style=\" margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><span style=\" font-family:'MS Shell Dlg 2'; color:#ffffff;\">HI THERE</span></p>\n"
        "<p style=\"-qt-paragraph-type:empty; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px; font-family:'MS Shell Dlg 2'; color:#ffffff;\"><br /></p>\n"
        "<p style=\" margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><span style=\" font-family:'MS Shell Dlg 2'; color:#ffffff;\">I WHISH YOU A PROFITABLE TRADE</span></p>\n"
        "<p style=\"-qt-paragraph-type:empty; mar"
                                "gin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px; font-family:'MS Shell Dlg 2'; color:#ffffff;\"><br /></p>\n"
        "<p style=\" margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><span style=\" font-family:'MS Shell Dlg 2'; color:#ffffff;\">VERSION 1 QT and 4 BCK</span></p></body></html>", None))
                self.label.setText(QCoreApplication.translate("MainWindow", "SYMBOLS", None))
                self.label_4.setText(QCoreApplication.translate("MainWindow", "OUTPUTS OPTIONS", None))
                self.label_9.setText(QCoreApplication.translate("MainWindow", "DAY = 800, WEEK = 900, MONTH = 1000", None))

        def calculation_TREND(self,esmm): 
                    
                    #for interv in inter:                      #get metatrader data for each name
                 
                esmm=str(esmm.upper())
                if ('USD') in esmm:
                        yf.pdr_override()
                        
                        namad = pdr.get_data_yahoo(esmm, period=(str(int(self.DAYSNUMBER.value()))+'d') ,interval='1D')
                        namad_panda = pd.DataFrame(namad,columns = ['Time','OPEN','HIGH','LOW','CLOSE','adj close','VOLUME'])
                        namad.reset_index(inplace=True)
                        namad_panda = namad.set_axis(['Time','OPEN','HIGH','LOW','CLOSE','adj close','VOLUME'], axis=1)
                        namad_panda['Time'] = namad_panda['Time'].apply(lambda a: datetime.datetime.strftime(a,"%Y-%m-%d %H:%M:%S"))
                        

                elif  ('SAF' in esmm) or ('SIL' in esmm) or ('ETC' in esmm) or ('طلا' in esmm) :
                    #    #print(self.out)
                      #  #print(self.time_frame_converter())
                        self.connect() 
                        ##print(self.days.value())
                        ##print(10*self.dayskala)
                        ##print(type(self.dayskala))
                        d = (self.DAYSNUMBER.value())*(1440/int(self.INTERVAL.value()))*10
                        ##print(int(d))
                        namad = mt5.copy_rates_from_pos(esmm, self.time_frame_converter_TR(),0,int(d))
                        namad_panda = pd.DataFrame(self.pandaa(namad),columns = ['Time','OPEN','HIGH','LOW','CLOSE','tVOLUME','Spread','VOLUME'])
                        ##print(namad_panda['Time'])
                        namad_panda['Time']=pd.to_datetime(namad_panda['Time'], unit='s')
                        ##print(namad_panda['date'],(namad_panda['hour']).split(":"))
                        namad_panda['hour'] = namad_panda['Time'].apply(lambda a: str(a).split(":")[0])
                        ##print(namad_panda['hour'])
                ##print(namad_panda['Time'])    
                #else: #print('esm symbol cherte',esmm)
                namad.size
               
                
                namad_panda_R = namad_panda[::-1]
               
                ###print("\n\n\n\n"+"             "+esmm+"\n\n\n\n" , namad_panda_R.head(10))
               
                out,newfinal,newfinal2 = self.cal_TREND(namad_panda['hour'],namad_panda['CLOSE'],namad_panda['HIGH'],namad_panda['LOW'],namad_panda['OPEN'],esmm,namad_panda['VOLUME'])
                namad_panda_R_2 = namad_panda_R[namad_panda_R.columns[[1,4]]]
                namad_panda_R_3 = namad_panda_R[namad_panda_R.columns[[1,2,3,4]]]
                
                newfinal = namad_panda_R_2.join(newfinal)
                newfinal2 = namad_panda_R_3.join(newfinal2)
                #mt5.shutdown()
                return newfinal2

        def calculation(self,esmm,trend):

                    #self.tinter = ['5m']  
                    
                    #for interv in inter:                      #get metatrader data for each name
                 
                esmm=str(esmm.upper())
                if ('USD') in esmm:
                        yf.pdr_override()
                        
                        namad = pdr.get_data_yahoo(esmm, period=(str(int(self.DAYSNUMBER.value()))+'d') ,interval='1D')
                        namad_panda = pd.DataFrame(namad,columns = ['Time','OPEN','HIGH','LOW','CLOSE','adj close','VOLUME'])
                        namad.reset_index(inplace=True)
                        namad_panda = namad.set_axis(['Time','OPEN','HIGH','LOW','CLOSE','adj close','VOLUME'], axis=1)
                        namad_panda['Time'] = namad_panda['Time'].apply(lambda a: datetime.datetime.strftime(a,"%Y-%m-%d %H:%M:%S"))

                elif  ('SAF' in esmm) or ('SIL' in esmm) or ('ETC' in esmm) or ('طلا' in esmm) :
                    #    #print(self.out)
                      #  #print(self.time_frame_converter())
                        #self.connect() 
                        ##print(self.days.value())
                        ##print(10*self.dayskala)
                        ##print(type(self.dayskala))
                        d = (self.DAYSNUMBER.value())*(1440/int(self.INTERVAL.value()))*10
                        ##print(int(d))
                        namad = mt5.copy_rates_from_pos(esmm, self.time_frame_converter(),0,int(d))
                        namad_panda = pd.DataFrame(self.pandaa(namad),columns = ['Time','OPEN','HIGH','LOW','CLOSE','tVOLUME','Spread','VOLUME'])
                        namad_panda['Time']=pd.to_datetime(namad_panda['Time'], unit='s')
                        namad_panda['hour'] = namad_panda['Time'].apply(lambda a: str(a).split(":")[0])
                        ##print(trend)
                    
                    
                #else: #print('esm symbol cherte',esmm)
                namad.size
               
                
                namad_panda_R = namad_panda[::-1]
               
                ###print("\n\n\n\n"+"             "+esmm+"\n\n\n\n" , namad_panda_R.head(10))
               
                out,newfinal,newfinal2,newfinal3 = self.cal(namad_panda['hour'],namad_panda['CLOSE'],namad_panda['HIGH'],namad_panda['LOW'],namad_panda['OPEN'],esmm,namad_panda['VOLUME'],trend)
                namad_panda_R_2 = namad_panda_R[namad_panda_R.columns[[0,1,4]]]
                namad_panda_R_3 = namad_panda_R[namad_panda_R.columns[[0,4]]]             
                              
                newfinal = namad_panda_R_2.join(newfinal)
                newfinal2 = namad_panda_R_3.join(newfinal2)
                newfinal3 = namad_panda_R_3.join(newfinal3)


                
                if self.excells:
                        with pd.ExcelWriter('RESULT'+str(esmm)+'.xlsx', mode="w", engine="xlsxwriter") as writer:
                                namad_panda_R.to_excel(writer, sheet_name = 'اطلاعات نماد'+esmm,index = False,freeze_panes=(1,0))
                                out.to_excel(writer, sheet_name = 'اندیکاتورها'+esmm,index=False,freeze_panes=(1,0))
                            # Auto-adjust columns' prop
                                form1 = writer.book.add_format()
                                form2 = writer.book.add_format()
                                form = writer.book.add_format()
                                form1.set_align('vcenter')
                                form1.set_align('center')
                                form2.set_align('vcenter')
                                form2.set_align('center')
                                form.set_font_color('white')
                                form.set_bg_color('green')                
                                
                                for column in namad_panda_R:
                                    column_width = max(namad_panda_R[column].astype(str).map(len).max()+3, len(column))
                                    col_idx = namad_panda_R.columns.get_loc(column)
                                    writer.sheets['اطلاعات نماد'+esmm].set_column(col_idx,col_idx, column_width,form1)
                                    
                                    
                                newfinal.to_excel(writer, sheet_name = 'تحلیل تایم فریم'+esmm,index=False,freeze_panes=(1,0))
                            # Auto-adjust columns' prop
                                writer.sheets['تحلیل تایم فریم'+esmm].set_column(3,8, None,form)

                                for column in newfinal:
                                    column_width = max(newfinal[column].astype(str).map(len).max()+10, len(column))
                                    col_idx = newfinal.columns.get_loc(column)
                                    writer.sheets['تحلیل تایم فریم'+esmm].set_column(col_idx,col_idx, column_width,form2)
                                
                                newfinal2.to_excel(writer, sheet_name = 'سیگنال تایم فریم'+esmm,index=False,freeze_panes=(1,0))
                            # Auto-adjust columns' prop
                                writer.sheets['سیگنال تایم فریم'+esmm].set_column(3,8, None,form)

                                for column in newfinal2:
                                    column_width = max(newfinal2[column].astype(str).map(len).max()+10, len(column))
                                    col_idx = newfinal2.columns.get_loc(column)
                                    writer.sheets['سیگنال تایم فریم'+esmm].set_column(col_idx,col_idx, column_width,form2)

                                newfinal3.to_excel(writer, sheet_name = 'نهایی'+esmm,index=False,freeze_panes=(1,0))
                            # Auto-adjust columns' prop
                                writer.sheets['نهایی'+esmm].set_column(3,8, None,form)

                                for column in newfinal3:
                                    column_width = max(newfinal3[column].astype(str).map(len).max()+10, len(column))
                                    col_idx = newfinal3.columns.get_loc(column)
                                    writer.sheets['نهایی'+esmm].set_column(col_idx,col_idx, column_width,form2)

                #KHOROJI.dfi.export('df.png')
                KHOROJImail = newfinal3.iloc[0:15,0:-1]
                KHOROJImail[esmm] = ''
                dfi.export(KHOROJImail.style.background_gradient(),esmm+'.png')
                
                

                
                    
                if self.whatsss:
                    KHOROJIwhats = newfinal3.iloc[0:5,0:-1]
                    #KHOROJIwhats[esmm] = ''
                    dfi.export(KHOROJIwhats.style.background_gradient(),esmm+'.png')
                    imagee = Image.open(esmm+'.png')
                    imagee = imagee.resize((imagee.width*10,imagee.height*10),Image.ADAPTIVE)
                    imagee.save(esmm+'bIG.png')
                    whatsappfilename = esmm+'bIG.png'
                    ##print(self.numbers)
                    pywhatkit.sendwhats_image(str(self.numbers), whatsappfilename,esmm,15,True,10)
                    os.remove(esmm+'bIG.png')
                    
                if self.piccs:
                    #ImageFile.LOAD_TRUNCATED_IMAGES = True
                    im = Image.open(esmm+'.png')
                    im.show()


                if self.emaills:
                    
                    mailfilename = esmm+'.png'
                    self.SendMail(mailfilename)

        def signal_TREND(self,data,close,openn,esmm):
            
                        data2 = pd.DataFrame(columns=['hour','STOCHRSI-K-SLOW','STOCHRSI-D-SLOW','STOCH-SIGNAL','CCI14','TREND-CCI14','CCI14-SIGNAL-based on 200','CCI14-SIGNAL-based on 180','CCI14-SIGNAL','TREND-based on 200','MACD','signal-macd','Histogram-macd','TREND-MACD','MACD-SIGNAL','TREND-MACD5','MACD-SIGNAL5','ADX','TREND-ADX','ADX-SIGNAL','DEMA','DEMA-SIGNAL'])
                        data2 = data2.merge(data, how='right')
                        data2 = pd.DataFrame(data2,columns=['hour','STOCHRSI-K-SLOW','STOCHRSI-D-SLOW','STOCH-SIGNAL','CCI14','CCI14-SIGNAL-based on 200','CCI14-SIGNAL-based on 180','TREND-CCI14','CCI14-SIGNAL','TREND-based on 200','MACD','signal-macd','Histogram-macd','TREND-MACD','MACD-SIGNAL','TREND-MACD5','MACD-SIGNAL5','ADX','TREND-ADX','ADX-SIGNAL','DEMA','DEMA-SIGNAL'])
                        final_signal=pd.DataFrame(columns=['hour','FINAL SIGNAL','CCI14-SIGNAL','CCI14-SIGNAL-based on 200','CCI14-SIGNAL-based on 180','STOCHSIGNAL','MACHINE SIGNAL','DELTA','Chikou','TREND POWER','TREND','REVENUE'])  
                        final_signal['hour']=data2['hour']
                        
                        TEMP_CCI = 'none'
                        TEMP_STOCH = "none"
                        TEMP_SIG = 'none'
                        price_TEMP_sell = 0
                        price_TEMP_BUY=0
                        LAST_CCI_200 = None
                        tempfinal = None
                        temp_final_etc = None
                        temp_final_usd = None
                        for i in range(1,len(data)):

                            count_BUY = 0
                            count_sell = 0

                            #CHIKOU
                            
                            if i > 26:
                                if close [i] > max(openn[i-26],close [i-26]):
                                        final_signal.loc[i,'Chikou'] = 'UPTREND'              
                                elif close [i] < min(openn[i-26],close [i-26]):
                                        final_signal.loc[i,'Chikou'] = 'DOWNTREND'    


                            #STOCH

                            if (data.loc[i,'STOCHRSI-K-SLOW'] < 20) and (data.loc[i,'STOCHRSI-D-SLOW'] < 20):
                                data2.loc[i,'STOCH-SIGNAL'] = 'Over Sold'
                            elif (data.loc[i,'STOCHRSI-K-SLOW'] > 80) and (data.loc[i,'STOCHRSI-D-SLOW'] > 80): 
                                    data2.loc[i,'STOCH-SIGNAL'] = 'Over Bought'

                            elif data.loc[i,'STOCHRSI-K-SLOW'] > data.loc[i,'STOCHRSI-D-SLOW']:
                                if (20 < data.loc[i,'STOCHRSI-D-SLOW']) and (20 > data.loc[(i-1),'STOCHRSI-D-SLOW']):
                                    
                                        data2.loc[i,'STOCH-SIGNAL'] = 'BUY'
                                        count_BUY = count_BUY + 1
                                        #data2.loc[j,'COUNT-BUY'] = count_BUY

                                        
                            elif data.loc[i,'STOCHRSI-K-SLOW'] < data.loc[i,'STOCHRSI-D-SLOW']:
                                    if (data.loc[i,'STOCHRSI-D-SLOW'] < 80) and (80 < data.loc[(i-1),'STOCHRSI-D-SLOW']):
                                                
                                        data2.loc[i,'STOCH-SIGNAL'] = 'SELL'
                                        count_sell = count_sell+1
                                        #data2.loc[i,'COUNT-SELL'] = count_sell

                                        
                            
                            else: data2.loc[i,'STOCH-SIGNAL'] = 'K and D are EQUAL'
                            
                            
                            #CCI14
                            
                            if data.loc[i,'CCI14'] > 100:
                                data2.loc[i,'TREND-CCI14'] = 'UPTREND'
                            elif data.loc[i,'CCI14'] < -100 :
                                data2.loc[i,'TREND-CCI14'] = 'DOWNTREND'
                            if (data.loc[i-1,'CCI14'] > 100) and (data.loc[i,'CCI14'] < 100 ):
                                    data2.loc[i,'CCI14-SIGNAL'] = 'SELL'
                                    count_sell = count_sell+1
                                    #data2.loc[i,'COUNT-SELL'] = count_sell
                            elif (data.loc[i-1,'CCI14'] < -100) and (data.loc[i,'CCI14'] > -100 ):
                                    data2.loc[i,'CCI14-SIGNAL'] = 'BUY'
                                    count_BUY = count_BUY + 1
                                    #data2.loc[i,'COUNT-BUY'] = count_BUY
                                #   if data.loc[i-1,'CCI14-SIGNAL'] == 'BUY':
                                #      data.loc[i,'CCI14-SIGNAL'] = 'BUY; KEEP GOING '
                                # else: data.loc[i,'CCI14-SIGNAL'] = 'BUY '


                            #CCI14-based on 200
                            
                            if data.loc[i,'CCI14'] > 200:
                                data2.loc[i,'TREND-based on 200'] = 'UPTREND'
                            elif data.loc[i,'CCI14'] < -200 :
                                data2.loc[i,'TREND-based on 200'] = 'DOWNTREND'
                            if ((data.loc[i-1,'CCI14'] > 200) and (data.loc[i,'CCI14'] < 200 )):
                                    data2.loc[i,'CCI14-SIGNAL-based on 200'] = 'SELL'
                                    count_sell = count_sell+1
                                    #data2.loc[i,'COUNT-SELL'] = count_sell
                            elif ((data.loc[i-1,'CCI14'] < -200) and (data.loc[i,'CCI14'] > -200 ) ):
                                    data2.loc[i,'CCI14-SIGNAL-based on 200'] = 'BUY'
                                    count_BUY = count_BUY + 1
                                    #data2.loc[i,'COUNT-BUY'] = count_BUY
                                #   if data.loc[i-1,'CCI14-SIGNAL'] == 'BUY':
                                #      data.loc[i,'CCI14-SIGNAL'] = 'BUY; KEEP GOING '
                                # else: data.loc[i,'CCI14-SIGNAL'] = 'BUY '


                            if data.loc[i,'CCI14'] > 180:
                                data2.loc[i,'TREND-based on 180'] = 'UPTREND'
                            elif data.loc[i,'CCI14'] < -180 :
                                data2.loc[i,'TREND-based on 180'] = 'DOWNTREND'
                            if ((data.loc[i-1,'CCI14'] > 180) and (data.loc[i,'CCI14'] < 180 )):
                                    data2.loc[i,'CCI14-SIGNAL-based on 180'] = 'SELL'
                                    count_sell = count_sell+1
                                    #data2.loc[i,'COUNT-SELL'] = count_sell
                            elif ((data.loc[i-1,'CCI14'] < -180) and (data.loc[i,'CCI14'] > -180 ) ):
                                    data2.loc[i,'CCI14-SIGNAL-based on 180'] = 'BUY'
                                    count_BUY = count_BUY + 1
                                    #data2.loc[i,'COUNT-BUY'] = count_BUY
                                #   if data.loc[i-1,'CCI14-SIGNAL'] == 'BUY':
                                #      data.loc[i,'CCI14-SIGNAL'] = 'BUY; KEEP GOING '
                                # else: data.loc[i,'CCI14-SIGNAL'] = 'BUY '
                            
                            
                            #MACD
                            
                            if (data.loc[i,'MACD'] > data.loc[i,'signal-macd']):
                                    if (data.loc[i,'MACD'] > 0) and (data.loc[i,'signal-macd'] > 0):
                                        data2.loc[i,'TREND-MACD'] = 'UPTREND'
                                    if (data.loc[i,'Histogram-macd'] > 0):
                                            data2.loc[i,'MACD-SIGNAL'] = 'BUY'
                                            count_BUY = count_BUY + 1
                                            #data2.loc[i,'COUNT-BUY'] = count_BUY
                            elif (data.loc[i,'MACD'] < data.loc[i,'signal-macd']):
                                    if (data.loc[i,'MACD'] < 0) and (data.loc[i,'signal-macd'] < 0):
                                            data2.loc[i,'TREND-MACD'] = 'DOWNTREND'
                                    if (data.loc[i,'Histogram-macd'] < 0):
                                            data2.loc[i,'MACD-SIGNAL'] = 'SELL'
                                            count_sell = count_sell+1
                                            #data2.loc[i,'COUNT-SELL'] = count_sell

                            
                            #MACD5
                            
                            if (data.loc[i,'MACD5'] > data.loc[i,'signal-macd5']):
                                    if (data.loc[i,'MACD5'] > 0) and (data.loc[i,'signal-macd5'] > 0):
                                        data2.loc[i,'TREND-MACD5'] = 'UPTREND'
                                    if (data.loc[i,'Histogram-macd5'] > 0):
                                            data2.loc[i,'MACD-SIGNAL5'] = 'BUY'
                                            count_BUY = count_BUY + 1
                                            #data2.loc[i,'COUNT-BUY'] = count_BUY
                            elif (data.loc[i,'MACD5'] < data.loc[i,'signal-macd5']):
                                    if (data.loc[i,'MACD5'] < 0) and (data.loc[i,'signal-macd5'] < 0):
                                            data2.loc[i,'TREND-MACD5'] = 'DOWNTREND'
                                    if (data.loc[i,'Histogram-macd5'] < 0):
                                            data2.loc[i,'MACD-SIGNAL5'] = 'SELL'
                                            count_sell = count_sell+1
                                            #data2.loc[i,'COUNT-SELL'] = count_sell
                            
                            #ADX      
                            
                            if data.loc[i,'ADX'] <= data.loc[(i-1),'ADX']:

                                    data2.loc[i,'TREND-ADX'] = 'WEAK TREND'
                            elif data.loc[i,'ADX'] > 20: 
                                if data.loc[i,'ADX'] > 40: 
                                    data2.loc[i,'TREND-ADX'] = 'GREAT TREND'
                                    
                                else: data2.loc[i,'TREND-ADX'] = 'GOOD TREND'
                                    
                            
                            if data.loc[i,'PLUS DI'] > data.loc[i,'MINUS DI'] :
                            
                                    if data.loc[i,'ADX'] > 20:
                                        if data.loc[i,'ADX'] > data.loc[(i-1),'ADX']:
                                            data2.loc[i,'ADX-SIGNAL'] = 'BUY'
                                            count_BUY = count_BUY + 1
                                        # data2.loc[i,'COUNT-BUY'] = count_BUY
                                        elif data.loc[i,'ADX'] <= data.loc[(i-1),'ADX']:

                                            data2.loc[i,'ADX-SIGNAL'] = 'BUY'
                                            count_BUY = count_BUY + 1
                                        # data2.loc[i,'COUNT-BUY'] = count_BUY
                                    else:  
                                        data2.loc[i,'ADX-SIGNAL'] = 'YELLOW WARNING'

                                

                            elif data.loc[i,'PLUS DI'] < data.loc[i,'MINUS DI'] :

                                    if data.loc[i,'ADX'] > 20:
                                        if data.loc[i,'ADX'] > data.loc[(i-1),'ADX']:
                                            data2.loc[i,'ADX-SIGNAL'] = 'SELL'
                                            count_sell = count_sell+1
                                        # data2.loc[i,'COUNT-SELL'] = count_sell
                                        elif data.loc[i,'ADX'] <= data.loc[(i-1),'ADX']:
                                            data2.loc[i,'ADX-SIGNAL'] = 'SELL'
                                            count_sell = count_sell+1
                                        # data2.loc[i,'COUNT-SELL'] = count_sell
                                    else: 
                                        data2.loc[i,'ADX-SIGNAL'] = 'YELLOW WARNING'

                                
                            else: data.loc[i,'ADX-SIGNAL'] = 'DI PLUS and DI MINUS are EQUAL'
                                
                            #DEMA
                            
                            if close[i] > data.loc[i,'DEMA']:
                                if openn[i] > data.loc[i,'DEMA']:
                                    data2.loc[i,'DEMA-SIGNAL'] = 'BUY'
                                    count_BUY = count_BUY + 1
                                # data2.loc[i,'COUNT-BUY'] = count_BUY
                                else:
                                    data2.loc[i,'DEMA-SIGNAL'] = 'احتیاط کن !! روند در حال تغییر است '
                            elif close[i] < data.loc[i,'DEMA']:
                                if openn[i] < data.loc[i,'DEMA']:
                                    data2.loc[i,'DEMA-SIGNAL'] = 'SELL'
                                    count_sell = count_sell+1
                                # data2.loc[i,'COUNT-SELL'] = count_sell
                                else: 
                                    data2.loc[i,'DEMA-SIGNAL'] = 'احتیاط کن !! روند در حال تغییر است'
                            
                            if 'SIL' in esmm:
                                    
                                ## FINAL SIGNAL SIL
                                
                                final_signal.loc[i,'STOCHSIGNAL'] = data2.loc[i,'STOCH-SIGNAL']
                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']
                                


                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                                if data2.loc[i,'TREND-MACD'] == 'DOWNTREND'or data2.loc[i,'TREND-MACD'] == 'UPTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD']

                                if data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']


                                if   data2.loc[i,'STOCH-SIGNAL'] == 'BUY' :
                                    if count_BUY > count_sell :
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - Delta: : '
                                elif data2.loc[i,'STOCH-SIGNAL'] == 'SELL' :
                                    if count_BUY < count_sell : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - Delta: '
                                else:
                                    if (count_BUY-count_sell) >=3 : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - NO STOCH - Delta:  '
                                    if (count_sell-count_BUY) >=3 : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - NO STOCH - Delta: '
                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell
                        
                            elif  ('<>' in esmm):
                                TEMP_STOCH = None #kesafat kari shod temp-stoch va b yekian ehtemalan badan baresi beshe
                                ## FINAL SIGNAL GOLD
                                final_signal.loc[i,'STOCHSIGNAL'] = data2.loc[i,'STOCH-SIGNAL']
                                b=i
                                if final_signal.STOCHSIGNAL.last_valid_index() != None:
                                    b = final_signal.STOCHSIGNAL.last_valid_index()
                                    

                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']
                            
                            
                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                            # if data2.loc[i,'TREND-MACD'] == 'DOWNTREND'or data2.loc[i,'TREND-MACD'] == 'UPTREND':
                                #    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD']

                                elif data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']
                                else : final_signal.loc[i,'TREND'] = None
                                
                                if  data2.loc[i,'ADX-SIGNAL'] == 'YELLOW WARNING':
                                    final_signal.loc[i,'MACHINE SIGNAL'] = "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning"     

                                elif data2.loc[i,'STOCH-SIGNAL'] == 'BUY' :
                                    TEMP_STOCH = 'BUY'
                                    if   (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                        if  (final_signal.loc[i,'TREND']=='DOWNTREND'): final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR BUY '
                                        elif ((count_BUY - count_sell) >= 2 ) :
                                            if (temp_final_usd == None) or (temp_final_usd == 'SELL'):
                                                final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                                temp_final_usd = 'BUY'

                                elif data2.loc[i,'STOCH-SIGNAL'] == 'SELL' :
                                    TEMP_STOCH = 'SELL'
                                    if (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                        if (final_signal.loc[i,'TREND']=='UPTREND'): final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR SELL '
                                        elif ((count_sell - count_BUY) >= 2 ) :
                                            if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                                final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                                temp_final_usd = 'SELL'

                                elif (TEMP_STOCH == 'BUY') and (final_signal.loc[i,'TREND']=='UPTREND') and (count_BUY-count_sell >=2 ) and (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                    if (temp_final_usd == None ) or (temp_final_usd == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        temp_final_usd = 'BUY'
                                elif (TEMP_STOCH == 'SELL') and (final_signal.loc[i,'TREND']=='DOWNTREND') and (count_BUY-count_sell <=2 ) and  (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                    if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        temp_final_usd = 'SELL'
                                

                                else: 
                                    """if final_signal.SIGNAL.last_valid_index() != None:
                                        a = final_signal.SIGNAL.last_valid_index()             

                                    if ((count_sell - count_BUY) >= 1 ) and (final_signal.loc[i,'TREND']=='DOWNTREND') and  final_signal['MACHINE SIGNAL'].loc[a] == 'BUY' or 'NOTICE FOR BUY':
                                        if (count_sell - count_BUY) >= 2  : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        else: final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE POSITION' 
                                        
                                    if ((count_BUY - count_sell) >= 1 ) and (final_signal.loc[i,'TREND']=='UPTREND') and final_signal['MACHINE SIGNAL'].loc[a] == 'SELL' or 'NOTICE FOR SELL':
                                        if (count_BUY - count_sell) >= 2  : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        else: final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE POSITION' """

                                    if final_signal['STOCHSIGNAL'].loc[b] == 'BUY' :
                                        if ((count_BUY - count_sell) >= 2 ):
                                            if final_signal.loc[i,'TREND']=='UPTREND' :
                                                if (temp_final_usd == None) or (temp_final_usd == 'SELL'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                                    temp_final_usd = 'BUY'
                                            elif (final_signal.loc[i,'TREND POWER'] =='GOOD TREND') or( final_signal.loc[i,'TREND POWER'] =='GREAT TREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE SELL POSITION'
                                        
                                        
                                    elif final_signal['STOCHSIGNAL'].loc[b] == 'SELL':
                                        if ((count_sell - count_BUY) >= 2 ):
                                            if final_signal.loc[i,'TREND']=='DOWNTREND' :
                                                if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                                    temp_final_usd = 'SELL'
                                            elif (final_signal.loc[i,'TREND POWER'] =='GOOD TREND') or( final_signal.loc[i,'TREND POWER'] =='GREAT TREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE BUY POSITON'
                                        
                                if (final_signal.loc[i,'TREND'] =='UPTREND') and (count_BUY-count_sell >=4 ) :
                                    if (temp_final_usd == None) or (temp_final_usd == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'    
                                        temp_final_usd = 'BUY'
                                #if (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold') or (data2.loc[i,'STOCH-SIGNAL']=='Over Bought') :
                                  #   final_signal.loc[i,'MACHINE SIGNAL'] = 'WAITING '
                                 #    temp_final_usd = 'waiting'

                                if (final_signal.loc[i,'TREND'] =='DOWNTREND') and (count_sell-count_BUY >=4 ) :
                                    if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'    
                                        temp_final_usd = 'SELL'
                                #if (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold') or (data2.loc[i,'STOCH-SIGNAL']=='Over Bought') : 
                                  #  final_signal.loc[i,'MACHINE SIGNAL'] = 'WAITING '
                                  #  temp_final_usd = 'waiting'

                                    
                             #   if temp_final_usd != None:
                              #      #print(i-1,'there')
                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell

                                                                ## REVENUE CALCULATING it not working properly when two sell or BUY signal come immideatly
                                if final_signal.loc[i,'MACHINE SIGNAL'] == 'SELL':
                                        price_TEMP_sell = close[i]
                                        if    price_TEMP_BUY != 0:
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                    
                                elif final_signal.loc[i,'MACHINE SIGNAL'] == 'BUY':
                                        price_TEMP_BUY = close[i] 
                                        if    price_TEMP_sell != 0:  
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY

                                                    
                            elif (('ETC') or ('طلا')) in esmm :
                                TEMP_STOCH = None #kesafat kari shod temp-stoch va b yekian ehtemalan badan baresi beshe
                                ## FINAL SIGNAL GOLD
                                final_signal.loc[i,'STOCHSIGNAL'] = data2.loc[i,'STOCH-SIGNAL']
                                b=i
                                if final_signal.STOCHSIGNAL.last_valid_index() != None:
                                    b = final_signal.STOCHSIGNAL.last_valid_index()
                                    #if b < i-15 : b=i
                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']
                            
                            
                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                            # if data2.loc[i,'TREND-MACD'] == 'DOWNTREND'or data2.loc[i,'TREND-MACD'] == 'UPTREND':
                                #    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD']

                                elif data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']
                                else : final_signal.loc[i,'TREND'] = None
                                
                                if  data2.loc[i,'ADX-SIGNAL'] == 'YELLOW WARNING':
                                    final_signal.loc[i,'MACHINE SIGNAL'] = ("OOPS CHECK ADX SIGNAL, IT's YELLOW Warning")

                                elif data2.loc[i,'STOCH-SIGNAL'] == 'BUY' :
                                    TEMP_STOCH = 'BUY'
                                    if   (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') and (final_signal.loc[i,'TREND']=='DOWNTREND'): final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR BUY '
                                    elif ((count_BUY - count_sell) >= 2 ) :
                                        if (temp_final_etc == None) or (temp_final_etc == 'SELL'):
                                            final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                            ##print(final_signal)
                                            temp_final_etc = 'BUY'

                                elif data2.loc[i,'STOCH-SIGNAL'] == 'SELL' :
                                    TEMP_STOCH = 'SELL'
                                    if (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') and (final_signal.loc[i,'TREND']=='UPTREND'): final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR SELL '
                                    elif ((count_sell - count_BUY) >= 2 ) :
                                        if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                            final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                            temp_final_etc = 'SELL'

                                elif (TEMP_STOCH == 'BUY') and (final_signal.loc[i,'TREND']=='UPTREND') and (count_BUY-count_sell >=2 ) :
                                    if (temp_final_etc == None ) or (temp_final_etc == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        temp_final_etc = 'BUY'
                                elif (TEMP_STOCH == 'SELL') and (final_signal.loc[i,'TREND']=='DOWNTREND') and (count_BUY-count_sell <=2 ) :
                                    if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        temp_final_etc = 'SELL'
                                

                                else: 
                                    """if final_signal.SIGNAL.last_valid_index() != None:
                                        a = final_signal.SIGNAL.last_valid_index()             

                                    if ((count_sell - count_BUY) >= 1 ) and (final_signal.loc[i,'TREND']=='DOWNTREND') and  final_signal['MACHINE SIGNAL'].loc[a] == 'BUY' or 'NOTICE FOR BUY':
                                        if (count_sell - count_BUY) >= 3  : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        else: final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE POSITION' 
                                        
                                    if ((count_BUY - count_sell) >= 1 ) and (final_signal.loc[i,'TREND']=='UPTREND') and final_signal['MACHINE SIGNAL'].loc[a] == 'SELL' or 'NOTICE FOR SELL':
                                        if (count_BUY - count_sell) >= 3  : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        else: final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE POSITION' """

                                    if final_signal['STOCHSIGNAL'].loc[b] == 'BUY' :
                                        if ((count_BUY - count_sell) >= 2 ):
                                            if final_signal.loc[i,'TREND']!='UPTREND' :
                                                if (temp_final_etc == None) or (temp_final_etc == 'SELL'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                                    temp_final_etc = 'BUY'
                                            elif (final_signal.loc[i,'TREND']!='UPTREND') and (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'NOTICE FOR BUY'
                                        
                                        
                                    elif final_signal['STOCHSIGNAL'].loc[b] == 'SELL':
                                        if ((count_sell - count_BUY) >= 2 ):
                                            if final_signal.loc[i,'TREND']=='DOWNTREND' :
                                                if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                                    temp_final_etc = 'SELL'
                                            elif (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'NOTICE FOR SELL'
                                        
                                if (final_signal.loc[i,'TREND'] =='UPTREND') and (count_BUY-count_sell >=4 ) :
                                    if (temp_final_etc == None) or (temp_final_etc == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'    
                                        temp_final_etc = 'BUY'
                                #if (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold') or (data2.loc[i,'STOCH-SIGNAL']=='Over Bought') :
                                  #   final_signal.loc[i,'MACHINE SIGNAL'] = 'WAITING '
                                 #    temp_final_etc = 'waiting'

                                if (final_signal.loc[i,'TREND'] =='DOWNTREND') and (count_sell-count_BUY >=4 ) :
                                    if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'    
                                        temp_final_etc = 'SELL'
                                #if (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold') or (data2.loc[i,'STOCH-SIGNAL']=='Over Bought') : 
                                  #  final_signal.loc[i,'MACHINE SIGNAL'] = 'WAITING '
                                  #  temp_final_etc = 'waiting'

                                    
                             #   if temp_final_etc != None:
                              #      #print(i-1,'there')
                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell

                                                                ## REVENUE CALCULATING it not working properly when two sell or BUY signal come immideatly
                                if final_signal.loc[i,'MACHINE SIGNAL'] == 'SELL':
                                        price_TEMP_sell = close[i]
                                        if    price_TEMP_BUY != 0:
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                    
                                elif final_signal.loc[i,'MACHINE SIGNAL'] == 'BUY':
                                        price_TEMP_BUY = close[i] 
                                        if    price_TEMP_sell != 0:  
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY

                                
                            
                                
                            
                            
                            elif ('SAF' or 'USD') in esmm:
                                TEMP_SIG = 'none'
                                #if i == 263:
                                #    #print(i , "NEAR")
                                
                                if data2.loc[i,'STOCH-SIGNAL'] == 'BUY' : TEMP_STOCH = 'BUY'
                                if data2.loc[i,'STOCH-SIGNAL'] == 'SELL' : TEMP_STOCH = 'SELL'

                                ## FINAL SIGNAL SAFFRON
                                final_signal.loc[i,'CCI14-SIGNAL'] = data2.loc[i,'CCI14-SIGNAL']
                                final_signal.loc[i,'CCI14-SIGNAL-based on 180'] = data2.loc[i,'CCI14-SIGNAL-based on 180']          
                                
                                


                                ## CALCULATING DELTA
                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']

                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                                if data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']
                            
                                if data2.loc[i,'CCI14-SIGNAL'] == 'BUY' :
                                    TEMP_CCI = 'BUY'
                                    if (count_BUY - count_sell) > 2 : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - WITHOUT STOCH'
                                    if ((count_sell > count_BUY) and (final_signal.loc[i,'TREND'] != 'UPTREND')):final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL, Notice For BUY'
                                
                                if data2.loc[i,'CCI14-SIGNAL'] == 'SELL' :
                                    TEMP_CCI = 'SELL'
                                    if (count_sell - count_BUY) > 2 : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - WITHOUT STOCH'
                                    elif (count_sell < count_BUY) and (final_signal.loc[i,'TREND'] != 'DOWNTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL, Notice For SELL'
                                if (TEMP_CCI == 'BUY') and (count_BUY-count_sell >= 4) and (final_signal.loc[i,'TREND'] == 'UPTREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - LAST CCI BUY'
                                if (TEMP_CCI == 'SELL') and (count_sell-count_BUY >= 4) and (final_signal.loc[i,'TREND'] == 'DOWNTREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - LAST CCI SELL'

                                if (TEMP_STOCH == 'BUY') and (TEMP_CCI == "BUY"):
                                    if ((count_BUY-count_sell >= 2) and (final_signal.loc[i,'TREND'] == 'UPTREND')) : 
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                    if (data2.loc[i,'TREND-ADX'] == 'WEAK TREND') and (final_signal.loc[i,'TREND'] != 'UPTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'ESLAH BAZAR'

                                if (TEMP_STOCH == 'SELL') and (TEMP_CCI == "SELL"):
                                    if ((count_BUY-count_sell <= 2) and (final_signal.loc[i,'TREND'] == 'DOWNTREND')) : 
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                    if (data2.loc[i,'TREND-ADX'] == 'WEAK TREND') and (final_signal.loc[i,'TREND'] != 'DOWNTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'ESLAH BAZAR'
                                
                                if (count_sell > count_BUY) and (data2.loc[i,'STOCH-SIGNAL'] == 'Over Bought'):
                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT - STOCH OVER BOUGHT'
                                    TEMP_SIG = 'WAIT - STOCH OVER BOUGHT'
                                if (TEMP_SIG == 'WAIT - STOCH OVER BOUGHT'):
                                        if (TEMP_CCI == 'SELL') and (TEMP_STOCH == 'SELL') and (count_BUY < count_sell) and (final_signal.loc[i,'TREND POWER'] == ('WEAK TREND')): final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        if (TEMP_CCI == 'SELL') and (TEMP_STOCH == 'SELL') and (count_BUY > count_sell) : final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT '
                                    #if (TEMP_CCI == 'SELL') and (TEMP_STOCH == 'SELL') and (count_BUY == count_sell) : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'

                                if (count_BUY > count_sell) and (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold'):
                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT - STOCH OVER SOLD'
                                    TEMP_SIG = 'WAIT - STOCH OVER SOLD'
                                if (TEMP_SIG == 'WAIT - STOCH OVER SOLD'):
                                        if (TEMP_CCI == 'BUY') and (TEMP_STOCH == 'BUY') and (count_BUY > count_sell) and  (final_signal.loc[i,'TREND POWER'] == ('WEAK TREND')) : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        if (TEMP_CCI == 'BUY') and (TEMP_STOCH == 'BUY') and (count_BUY < count_sell) : final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT '
                                

                                if (data2.loc[i,'CCI14-SIGNAL'] == 'BUY') and (final_signal.loc[i,'TREND POWER'] == ('GOOD' or 'GREAT')) and ((final_signal.loc[i,'TREND'] == 'DOWNTREND') or (final_signal.loc[i+1,'TREND'] == 'DOWNTREND')): final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL'
                                if (data2.loc[i,'CCI14-SIGNAL'] == 'SELL') and (final_signal.loc[i,'TREND POWER'] == ('GOOD' or 'GREAT')) and ((final_signal.loc[i,'TREND'] == 'UPTREND') or (final_signal.loc[i+1,'TREND'] == 'UPTREND')): final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL'    
                                
                                if  data2.loc[i,'ADX-SIGNAL'] == 'YELLOW WARNING':
                                    final_signal.loc[i,'MACHINE SIGNAL'] = "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning"
                                    
                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell
                                
                                
                            


                                if ((LAST_CCI_200 == 'BUY') or (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'BUY')):
                                
                                    if (final_signal.loc[i,'Chikou'] == 'UPTREND'):
                                        #if tempfinal != 'BUY':
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR BUY'
                                            #tempfinal = 'BUY'
                                    
                                    #if ((final_signal.loc[i,'MACHINE SIGNAL']=='BUY - WITHOUT STOCH' )):
                                            
                                    #            final_signal.loc[i,'FINAL SIGNAL'] = 'BUY IS AN OPTION'
                                                
                                    
                                    if (TEMP_STOCH == 'BUY'):
                                        if (final_signal.loc[i,'MACHINE SIGNAL']=='BUY - LAST CCI BUY'):
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR BUY' 

                                        if (((final_signal.loc[i,'MACHINE SIGNAL'] == "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning") and (count_BUY-count_sell>=3)) or (final_signal.loc[i,'MACHINE SIGNAL']=='BUY' )):
                                            if tempfinal != 'BUY':
                                                final_signal.loc[i,'FINAL SIGNAL'] = 'BUY'
                                                tempfinal = 'BUY'
                                    
                                

                                                

                                if ((LAST_CCI_200 == 'sell') or (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'SELL')):
                                    ##print(final_signal.loc[i,'MACHINE SIGNAL'])
                                    if (final_signal.loc[i,'Chikou'] == 'DOWNTREND'):
                                       # if tempfinal != 'sell':
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR SELL'
                                        #    tempfinal = 'sell'
                                    #if ((final_signal.loc[i,'MACHINE SIGNAL']=='SELL - WITHOUT STOCH' )):
                                            
                                    #            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR SELL'
                                            

                                    if (TEMP_STOCH == 'SELL'):
                                        if (final_signal.loc[i,'MACHINE SIGNAL']=='SELL - LAST CCI SELL'):
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR SELL' 

                                        if (((final_signal.loc[i,'MACHINE SIGNAL'] == "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning") and (count_sell-count_BUY>=3)) or (final_signal.loc[i,'MACHINE SIGNAL']=='SELL' ) ):
                                            if tempfinal != 'sell':
                                                final_signal.loc[i,'FINAL SIGNAL'] = 'SELL'
                                                tempfinal = 'sell'                         


                                    

                                    

                                if (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'SELL'):
                                    LAST_CCI_200 = 'sell'
                                if (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'BUY'):
                                    LAST_CCI_200 = 'BUY' 
                                
                                
                                ## REVENUE CALCULATING it not working properly when two sell or BUY signal come immideatly
                                if final_signal.loc[i,'FINAL SIGNAL'] == 'SELL':
                                        price_TEMP_sell = close[i]
                                        if    price_TEMP_BUY != 0:
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                    
                                elif final_signal.loc[i,'FINAL SIGNAL'] == 'BUY':
                                        price_TEMP_BUY = close[i] 
                                        if    price_TEMP_sell != 0:  
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                            
                        
                        final_signal['STOCHSIGNAL'] = data2['STOCH-SIGNAL']
                        #final_signal.loc[,'SUM-REVENUE'] = final_signal['REVENUE'].sum()
                        
                        final_signal_print = final_signal
                        final_signal_print.loc[i,'REVENUE'] =  final_signal_print['REVENUE'].sum()
                        del  final_signal_print['COUNT-BUY']
                        del  final_signal_print['COUNT- SELL']
                        del  final_signal_print['CCI14-SIGNAL']
                        final_signal_print.dropna(how='all', axis=1, inplace=True)
                        if 'TREND POWER' not in final_signal_print.columns:
                            final_signal_print['TREND POWER'] = pd.Series([])
                        return data2,final_signal_print
               
        def signal(self,data,close,openn,esmm,trend):
                        
                        data2 = pd.DataFrame(columns=['hour','STOCHRSI-K-SLOW','STOCHRSI-D-SLOW','STOCH-SIGNAL','CCI14','TREND-CCI14','CCI14-SIGNAL-based on 200','CCI14-SIGNAL-based on 180','CCI14-SIGNAL','TREND-based on 200','MACD','signal-macd','Histogram-macd','TREND-MACD','MACD-SIGNAL','TREND-MACD5','MACD-SIGNAL5','ADX','TREND-ADX','ADX-SIGNAL','DEMA','DEMA-SIGNAL'])
                        data2 = data2.merge(data, how='right')
                        data2 = pd.DataFrame(data2,columns=['hour','STOCHRSI-K-SLOW','STOCHRSI-D-SLOW','STOCH-SIGNAL','CCI14','CCI14-SIGNAL-based on 200','CCI14-SIGNAL-based on 180','TREND-CCI14','CCI14-SIGNAL','TREND-based on 200','MACD','signal-macd','Histogram-macd','TREND-MACD','MACD-SIGNAL','TREND-MACD5','MACD-SIGNAL5','ADX','TREND-ADX','ADX-SIGNAL','DEMA','DEMA-SIGNAL'])
                        final_signal=pd.DataFrame(columns=['FINAL SIGNAL','CCI14-SIGNAL','CCI14-SIGNAL-based on 200','CCI14-SIGNAL-based on 180','STOCHSIGNAL','MACHINE SIGNAL','DELTA','Chikou','TREND POWER','TREND','REVENUE'])  
                        final_signal_overal=pd.DataFrame(columns=['Machine Signal'+'-'+self.timefr,'Machine Signal'+'-'+self.timefrTR,'Delta'+'-'+self.timefrTR,'Power Trend'+'-'+self.timefrTR,'Trend'+'-'+self.timefrTR,'OVERAL REVENUE','OVERAL SIGNAL','WINRATE'])  
                        trednd = trend.add_suffix('-'+self.timefrTR)
                        trednd = trednd.rename(columns={'hour'+'-'+self.timefrTR: 'hour'})
                        trednd = trednd[::-1]
                        data2 = pd.merge(data2,trednd,how='outer',on='hour')
                        TEMP_CCI = 'none'
                        TEMP_STOCH = "none"
                        TEMP_SIG = 'none'
                        price_TEMP_sell = 0
                        price_TEMP_BUY=0
                        price_TEMP_sell_machin = 0
                        price_TEMP_BUY_machin=0
                        price_TEMP_close_sell = 0
                        price_TEMP_close_buy = 0
                        LAST_CCI_200 = None
                        tempfinal = None
                        temp_final_etc = None
                        temp_final_usd = None
                        win = 0
                        loss = 0
                        win_overal = 0
                        loss_overal = 0
                        lossindex = 0.009
                        temp_final_etc_overal = None
                        candel_counter = None
                        priceclose = None
                        priceclosetemp = None
                        for i in range(1,len(data)):

                            count_BUY = 0
                            count_sell = 0

                            #CHIKOU
                            
                            if i > 26:
                                if close [i] > max(openn[i-26],close [i-26]):
                                        final_signal.loc[i,'Chikou'] = 'UPTREND'              
                                elif close [i] < min(openn[i-26],close [i-26]):
                                        final_signal.loc[i,'Chikou'] = 'DOWNTREND'    

                            #STOCH

                            if (data.loc[i,'STOCHRSI-K-SLOW'] < 20) and (data.loc[i,'STOCHRSI-D-SLOW'] < 20):
                                data2.loc[i,'STOCH-SIGNAL'] = 'Over Sold'
                            elif (data.loc[i,'STOCHRSI-K-SLOW'] > 80) and (data.loc[i,'STOCHRSI-D-SLOW'] > 80): 
                                    data2.loc[i,'STOCH-SIGNAL'] = 'Over Bought'
                            elif data.loc[i,'STOCHRSI-K-SLOW'] > data.loc[i,'STOCHRSI-D-SLOW']:
                                if (20 < data.loc[i,'STOCHRSI-D-SLOW']) and (20 > data.loc[(i-1),'STOCHRSI-D-SLOW']):
                                    
                                        data2.loc[i,'STOCH-SIGNAL'] = 'BUY'
                                        count_BUY = count_BUY + 1                                        
                            elif data.loc[i,'STOCHRSI-K-SLOW'] < data.loc[i,'STOCHRSI-D-SLOW']:
                                    if (data.loc[i,'STOCHRSI-D-SLOW'] < 80) and (80 < data.loc[(i-1),'STOCHRSI-D-SLOW']):
                                                
                                        data2.loc[i,'STOCH-SIGNAL'] = 'SELL'
                                        count_sell = count_sell+1
                            else: data2.loc[i,'STOCH-SIGNAL'] = 'K and D are EQUAL'                            
                            #CCI14
                            if data.loc[i,'CCI14'] > 100:
                                data2.loc[i,'TREND-CCI14'] = 'UPTREND'
                            elif data.loc[i,'CCI14'] < -100 :
                                data2.loc[i,'TREND-CCI14'] = 'DOWNTREND'
                            if (data.loc[i-1,'CCI14'] > 100) and (data.loc[i,'CCI14'] < 100 ):
                                    data2.loc[i,'CCI14-SIGNAL'] = 'SELL'
                                    count_sell = count_sell+1
                            elif (data.loc[i-1,'CCI14'] < -100) and (data.loc[i,'CCI14'] > -100 ):
                                    data2.loc[i,'CCI14-SIGNAL'] = 'BUY'
                                    count_BUY = count_BUY + 1
                            #CCI14-based on 200
                            
                            if data.loc[i,'CCI14'] > 200:
                                data2.loc[i,'TREND-based on 200'] = 'UPTREND'
                            elif data.loc[i,'CCI14'] < -200 :
                                data2.loc[i,'TREND-based on 200'] = 'DOWNTREND'
                            if ((data.loc[i-1,'CCI14'] > 200) and (data.loc[i,'CCI14'] < 200 )):
                                    data2.loc[i,'CCI14-SIGNAL-based on 200'] = 'SELL'
                                    count_sell = count_sell+1
                            elif ((data.loc[i-1,'CCI14'] < -200) and (data.loc[i,'CCI14'] > -200 ) ):
                                    data2.loc[i,'CCI14-SIGNAL-based on 200'] = 'BUY'
                                    count_BUY = count_BUY + 1

                            if data.loc[i,'CCI14'] > 180:
                                data2.loc[i,'TREND-based on 180'] = 'UPTREND'
                            elif data.loc[i,'CCI14'] < -180 :
                                data2.loc[i,'TREND-based on 180'] = 'DOWNTREND'
                            if ((data.loc[i-1,'CCI14'] > 180) and (data.loc[i,'CCI14'] < 180 )):
                                    data2.loc[i,'CCI14-SIGNAL-based on 180'] = 'SELL'
                                    count_sell = count_sell+1
                                
                            elif ((data.loc[i-1,'CCI14'] < -180) and (data.loc[i,'CCI14'] > -180 ) ):
                                    data2.loc[i,'CCI14-SIGNAL-based on 180'] = 'BUY'
                                    count_BUY = count_BUY + 1
                                                            
                            #MACD
                            
                            if (data.loc[i,'MACD'] > data.loc[i,'signal-macd']):
                                    if (data.loc[i,'MACD'] > 0) and (data.loc[i,'signal-macd'] > 0):
                                        data2.loc[i,'TREND-MACD'] = 'UPTREND'
                                    if (data.loc[i,'Histogram-macd'] > 0):
                                            data2.loc[i,'MACD-SIGNAL'] = 'BUY'
                                            count_BUY = count_BUY + 1
                                
                            elif (data.loc[i,'MACD'] < data.loc[i,'signal-macd']):
                                    if (data.loc[i,'MACD'] < 0) and (data.loc[i,'signal-macd'] < 0):
                                            data2.loc[i,'TREND-MACD'] = 'DOWNTREND'
                                    if (data.loc[i,'Histogram-macd'] < 0):
                                            data2.loc[i,'MACD-SIGNAL'] = 'SELL'
                                            count_sell = count_sell+1
                                                        
                            #MACD5
                            
                            if (data.loc[i,'MACD5'] > data.loc[i,'signal-macd5']):
                                    if (data.loc[i,'MACD5'] > 0) and (data.loc[i,'signal-macd5'] > 0):
                                        data2.loc[i,'TREND-MACD5'] = 'UPTREND'
                                    if (data.loc[i,'Histogram-macd5'] > 0):
                                            data2.loc[i,'MACD-SIGNAL5'] = 'BUY'
                                            count_BUY = count_BUY + 1
                            
                            elif (data.loc[i,'MACD5'] < data.loc[i,'signal-macd5']):
                                    if (data.loc[i,'MACD5'] < 0) and (data.loc[i,'signal-macd5'] < 0):
                                            data2.loc[i,'TREND-MACD5'] = 'DOWNTREND'
                                    if (data.loc[i,'Histogram-macd5'] < 0):
                                            data2.loc[i,'MACD-SIGNAL5'] = 'SELL'
                                            count_sell = count_sell+1
                            
                            #ADX      
                            
                            if data.loc[i,'ADX'] <= data.loc[(i-1),'ADX']:

                                    data2.loc[i,'TREND-ADX'] = 'WEAK TREND'
                            elif data.loc[i,'ADX'] > 20: 
                                if data.loc[i,'ADX'] > 40: 
                                    data2.loc[i,'TREND-ADX'] = 'GREAT TREND'
                                    
                                else: data2.loc[i,'TREND-ADX'] = 'GOOD TREND'                              
                            if data.loc[i,'PLUS DI'] > data.loc[i,'MINUS DI'] :
                            
                                    if data.loc[i,'ADX'] > 20:
                                        if data.loc[i,'ADX'] > data.loc[(i-1),'ADX']:
                                            data2.loc[i,'ADX-SIGNAL'] = 'BUY'
                                            count_BUY = count_BUY + 1
                                        # data2.loc[i,'COUNT-BUY'] = count_BUY
                                        elif data.loc[i,'ADX'] <= data.loc[(i-1),'ADX']:

                                            data2.loc[i,'ADX-SIGNAL'] = 'BUY'
                                            count_BUY = count_BUY + 1
                                        # data2.loc[i,'COUNT-BUY'] = count_BUY
                                    else:  
                                        data2.loc[i,'ADX-SIGNAL'] = 'YELLOW WARNING'
                            elif data.loc[i,'PLUS DI'] < data.loc[i,'MINUS DI'] :

                                    if data.loc[i,'ADX'] > 20:
                                        if data.loc[i,'ADX'] > data.loc[(i-1),'ADX']:
                                            data2.loc[i,'ADX-SIGNAL'] = 'SELL'
                                            count_sell = count_sell+1
                                        # data2.loc[i,'COUNT-SELL'] = count_sell
                                        elif data.loc[i,'ADX'] <= data.loc[(i-1),'ADX']:
                                            data2.loc[i,'ADX-SIGNAL'] = 'SELL'
                                            count_sell = count_sell+1
                                        # data2.loc[i,'COUNT-SELL'] = count_sell
                                    else: 
                                        data2.loc[i,'ADX-SIGNAL'] = 'YELLOW WARNING'       
                            else: data.loc[i,'ADX-SIGNAL'] = 'DI PLUS and DI MINUS are EQUAL'
                                
                            #DEMA
                            
                            if close[i] > data.loc[i,'DEMA']:
                                if openn[i] > data.loc[i,'DEMA']:
                                    data2.loc[i,'DEMA-SIGNAL'] = 'BUY'
                                    count_BUY = count_BUY + 1
                                
                                else:
                                    data2.loc[i,'DEMA-SIGNAL'] = 'احتیاط کن !! روند در حال تغییر است '
                            elif close[i] < data.loc[i,'DEMA']:
                                if openn[i] < data.loc[i,'DEMA']:
                                    data2.loc[i,'DEMA-SIGNAL'] = 'SELL'
                                    count_sell = count_sell+1
                                
                                else: 
                                    data2.loc[i,'DEMA-SIGNAL'] = 'احتیاط کن !! روند در حال تغییر است'
                            
                            
                            
                            if 'SIL' in esmm:
                                    
                                ## FINAL SIGNAL SIL
                                
                                final_signal.loc[i,'STOCHSIGNAL'] = data2.loc[i,'STOCH-SIGNAL']
                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']
                                


                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                                if data2.loc[i,'TREND-MACD'] == 'DOWNTREND'or data2.loc[i,'TREND-MACD'] == 'UPTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD']

                                if data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']


                                if   data2.loc[i,'STOCH-SIGNAL'] == 'BUY' :
                                    if count_BUY > count_sell :
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - Delta: : '
                                elif data2.loc[i,'STOCH-SIGNAL'] == 'SELL' :
                                    if count_BUY < count_sell : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - Delta: '
                                else:
                                    if (count_BUY-count_sell) >=3 : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - NO STOCH - Delta:  '
                                    if (count_sell-count_BUY) >=3 : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - NO STOCH - Delta: '
                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell
                        
                            elif  ('<>' in esmm):
                                TEMP_STOCH = None #kesafat kari shod temp-stoch va b yekian ehtemalan badan baresi beshe
                                ## FINAL SIGNAL GOLD
                                final_signal.loc[i,'STOCHSIGNAL'] = data2.loc[i,'STOCH-SIGNAL']
                                b=i
                                if final_signal.STOCHSIGNAL.last_valid_index() != None:
                                    b = final_signal.STOCHSIGNAL.last_valid_index()
                                    

                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']
                            
                            
                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                            # if data2.loc[i,'TREND-MACD'] == 'DOWNTREND'or data2.loc[i,'TREND-MACD'] == 'UPTREND':
                                #    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD']

                                elif data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']
                                else : final_signal.loc[i,'TREND'] = None
                                
                                if  data2.loc[i,'ADX-SIGNAL'] == 'YELLOW WARNING':
                                    
                                    final_signal.loc[i,'MACHINE SIGNAL'] = "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning"     

                                if data2.loc[i,'STOCH-SIGNAL'] == 'BUY' :
                                    TEMP_STOCH = 'BUY'
                                    if   (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                        if  (final_signal.loc[i,'TREND']=='DOWNTREND'): final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR BUY '
                                        elif ((count_BUY - count_sell) >= 2 ) :
                                            if (temp_final_usd == None) or (temp_final_usd == 'SELL'):
                                                final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                              
                                                temp_final_usd = 'BUY'

                                elif data2.loc[i,'STOCH-SIGNAL'] == 'SELL' :
                                    TEMP_STOCH = 'SELL'
                                    if (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                        if (final_signal.loc[i,'TREND']=='UPTREND'): final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR SELL '
                                        elif ((count_sell - count_BUY) >= 2 ) :
                                            if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                                final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                                temp_final_usd = 'SELL'

                                elif (TEMP_STOCH == 'BUY') and (final_signal.loc[i,'TREND']=='UPTREND') and (count_BUY-count_sell >=2 ) and (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                    if (temp_final_usd == None ) or (temp_final_usd == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        temp_final_usd = 'BUY'
                                elif (TEMP_STOCH == 'SELL') and (final_signal.loc[i,'TREND']=='DOWNTREND') and (count_BUY-count_sell <=2 ) and  (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                    if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        temp_final_usd = 'SELL'
                                

                                else: 
                                    """if final_signal.SIGNAL.last_valid_index() != None:
                                        a = final_signal.SIGNAL.last_valid_index()             

                                    if ((count_sell - count_BUY) >= 1 ) and (final_signal.loc[i,'TREND']=='DOWNTREND') and  final_signal['MACHINE SIGNAL'].loc[a] == 'BUY' or 'NOTICE FOR BUY':
                                        if (count_sell - count_BUY) >= 2  : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        else: final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE POSITION' 
                                        
                                    if ((count_BUY - count_sell) >= 1 ) and (final_signal.loc[i,'TREND']=='UPTREND') and final_signal['MACHINE SIGNAL'].loc[a] == 'SELL' or 'NOTICE FOR SELL':
                                        if (count_BUY - count_sell) >= 2  : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        else: final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE POSITION' """

                                    if final_signal['STOCHSIGNAL'].loc[b] == 'BUY' :
                                        if ((count_BUY - count_sell) >= 2 ):
                                            if final_signal.loc[i,'TREND']=='UPTREND' :
                                                if (temp_final_usd == None) or (temp_final_usd == 'SELL'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                                    temp_final_usd = 'BUY'
                                            elif (final_signal.loc[i,'TREND POWER'] =='GOOD TREND') or( final_signal.loc[i,'TREND POWER'] =='GREAT TREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE SELL POSITION'
                                        
                                        
                                    elif final_signal['STOCHSIGNAL'].loc[b] == 'SELL':
                                        if ((count_sell - count_BUY) >= 2 ):
                                            if final_signal.loc[i,'TREND']=='DOWNTREND' :
                                                if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                                    temp_final_usd = 'SELL'
                                            elif (final_signal.loc[i,'TREND POWER'] =='GOOD TREND') or( final_signal.loc[i,'TREND POWER'] =='GREAT TREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'CLOSE BUY POSITON'
                                        
                                if (final_signal.loc[i,'TREND'] =='UPTREND') and (count_BUY-count_sell >=4 ) :
                                    if (temp_final_usd == None) or (temp_final_usd == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'    
                                        temp_final_usd = 'BUY'
                                #if (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold') or (data2.loc[i,'STOCH-SIGNAL']=='Over Bought') :
                                  #   final_signal.loc[i,'MACHINE SIGNAL'] = 'WAITING '
                                 #    temp_final_usd = 'waiting'

                                if (final_signal.loc[i,'TREND'] =='DOWNTREND') and (count_sell-count_BUY >=4 ) :
                                    if (temp_final_usd == None) or (temp_final_usd == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'    
                                        temp_final_usd = 'SELL'
                                #if (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold') or (data2.loc[i,'STOCH-SIGNAL']=='Over Bought') : 
                                  #  final_signal.loc[i,'MACHINE SIGNAL'] = 'WAITING '
                                  #  temp_final_usd = 'waiting'

                                    
                             #   if temp_final_usd != None:
                              #      #print(i-1,'there')
                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell

                                                                ## REVENUE CALCULATING it not working properly when two sell or BUY signal come immideatly
                                if final_signal.loc[i,'MACHINE SIGNAL'] == 'SELL':
                                        price_TEMP_sell = close[i]
                                        if    price_TEMP_BUY != 0:
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                    
                                elif final_signal.loc[i,'MACHINE SIGNAL'] == 'BUY':
                                        price_TEMP_BUY = close[i] 
                                        if    price_TEMP_sell != 0:  
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                                    
                            elif  (('ETC') or ('طلا') or ('GB')) in esmm :

                                final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefrTR] = data2.loc[i,'MACHINE SIGNAL'+'-'+self.timefrTR]
                                final_signal_overal.loc[i,'Delta'+'-'+self.timefrTR] = data2.loc[i,'DELTA'+'-'+self.timefrTR]
                                final_signal_overal.loc[i,'Power Trend'+'-'+self.timefrTR] = data2.loc[i,'TREND POWER'+'-'+self.timefrTR]
                                final_signal_overal.loc[i,'Trend'+'-'+self.timefrTR] = data2.loc[i,'TREND'+'-'+self.timefrTR]

                                
                                TEMP_STOCH = None #kesafat kari shod temp-stoch va b yekian ehtemalan badan baresi beshe
                                ## FINAL SIGNAL GOLD
                                final_signal.loc[i,'STOCHSIGNAL'] = data2.loc[i,'STOCH-SIGNAL']
                                b=i
                                if final_signal.STOCHSIGNAL.last_valid_index() != None:
                                    b = final_signal.STOCHSIGNAL.last_valid_index()
                                    #if b < i-15 : b=i
                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']
                            
                            
                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                            
                                elif data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']
                                else : final_signal.loc[i,'TREND'] = None
                                
                                if  data2.loc[i,'ADX-SIGNAL'] == 'YELLOW WARNING':
                                    final_signal.loc[i,'MACHINE SIGNAL'] = ("OOPS CHECK ADX SIGNAL, IT's YELLOW Warning")
                                    final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = ("OOPS CHECK ADX SIGNAL, IT's YELLOW Warning")

                                if data2.loc[i,'STOCH-SIGNAL'] == 'BUY' :
                                    TEMP_STOCH = 'BUY'
                                    if   (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') and (final_signal.loc[i,'TREND']=='DOWNTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR BUY '
                                        final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'SLEEP ON IT, NOTICE FOR BUY '

                                    elif ((count_BUY - count_sell) >= 2 ) :
                                        if (temp_final_etc == None) or (temp_final_etc == 'SELL'):
                                            final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'BUY'
                                            temp_final_etc = 'BUY'
                                            



                                        
                                            ##print(data2.loc[i,'TREND'+'-'+self.timefrTR])
                                            ##print(data2.loc[i,'DELTA'+'-'+self.timefrTR])
                                            ##print(data2.loc[i,'TREND POWER'+'-'+self.timefrTR])

                                            
                                                        
                                            #elif (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == ( 'WEAK TREND')):
                                            #    if ((data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  2') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  3') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  4')):
                                            #        final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'NOTICE FOR BUY'
                                            #        candelcounter = i+6
                                            #        pricecpunter = close[i]

                                              #if ternd delta movafeq va bozogtarmosavi 2 trend up trend ya to sell downtrend 
                                                #if not ta akhar rooz harvaqt trend movafeq shod va deltal movaq ya sefr shod signal BUY bede 
                                            ##print(final_signal)
                                            

                                elif data2.loc[i,'STOCH-SIGNAL'] == 'SELL' :
                                    TEMP_STOCH = 'SELL'
                                    if (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') and (final_signal.loc[i,'TREND']=='UPTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SLEEP ON IT, NOTICE FOR SELL '
                                        final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'SLEEP ON IT, NOTICE FOR SELL'
                                    elif ((count_sell - count_BUY) >= 2 ) :
                                        if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                            final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'SELL'
                                            temp_final_etc = 'SELL'
                                                                                       
                                            

                                            #elif (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == ( 'WEAK TREND')):
                                                #if ((data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'SELL  2') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'SELL  3') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'SELL  4')):
                                                #    final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'NOTICE FOR SELL'
                                                #    candelcounter = i+6
                                                #    pricecpunter = close[i]
                                           

                                elif (TEMP_STOCH == 'BUY') and (final_signal.loc[i,'TREND']=='UPTREND') and (count_BUY-count_sell >=2 ) :
                                    if (temp_final_etc == None ) or (temp_final_etc == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'BUY'
                                        temp_final_etc = 'BUY'
                                        

                                        
                                #elif (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == ( 'WEAK TREND')):
                                 #       if ((data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  2') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  3') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  4')):
                                  #          final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'NOTICE FOR BUY'
                                   #         candelcounter = i+6
                                    #        pricecpunter = close[i]    
                                    #                                    
                                elif (TEMP_STOCH == 'SELL') and (final_signal.loc[i,'TREND']=='DOWNTREND') and (count_BUY-count_sell <=2 ) :
                                    if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'SELL'
                                        temp_final_etc = 'SELL'
                                        

                                                                 

                                else: 

                                    if final_signal['STOCHSIGNAL'].loc[b] == 'BUY' :
                                        if ((count_BUY - count_sell) >= 2 ):
                                            if final_signal.loc[i,'TREND']!='UPTREND' :
                                                if (temp_final_etc == None) or (temp_final_etc == 'SELL'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                                    final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'BUY'
                                                    temp_final_etc = 'BUY'  
                                                                                              

                                            elif (final_signal.loc[i,'TREND']!='UPTREND') and (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                                final_signal.loc[i,'MACHINE SIGNAL'] = 'NOTICE FOR BUY'
                                                final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'NOTICE FOR BUY'
                                        
                                        
                                    elif final_signal['STOCHSIGNAL'].loc[b] == 'SELL':
                                        if ((count_sell - count_BUY) >= 2 ):
                                            if final_signal.loc[i,'TREND']=='DOWNTREND' :
                                                if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                                    final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'SELL'
                                                    temp_final_etc = 'SELL'
                                                    

                                                    
                                            elif (final_signal.loc[i,'TREND POWER'] =='GOOD TREND' or 'GREAT TREND') :
                                                final_signal.loc[i,'MACHINE SIGNAL'] = 'NOTICE FOR SELL'
                                                final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'NOTICE FOR SELL'
                                        
                                if (final_signal.loc[i,'TREND'] =='UPTREND') and (count_BUY-count_sell >=4 ) :
                                    if (temp_final_etc == None) or (temp_final_etc == 'SELL'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'    
                                        final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'BUY'
                                        temp_final_etc = 'BUY'
                                        
                                       

                                if (final_signal.loc[i,'TREND'] =='DOWNTREND') and (count_sell-count_BUY >=4 ) :
                                    if (temp_final_etc == None) or (temp_final_etc == 'BUY'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'    
                                        final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'SELL'
                                        temp_final_etc = 'SELL'
                                        

                                temp_final_etc_jadid = temp_final_etc   
                                
                                ## OVERAL CALCULATION 
                                if final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] == 'SELL':

                                    if (data2.loc[i,'TREND'+'-'+self.timefrTR] == 'DOWNTREND') :
                                        if ((data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'SELL  2') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'SELL  3') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'SELL  4')):
                                            if ((data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == 'GOOD TREND') or (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == 'GREAT TREND') or (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == 'WEAK TREND')):
                                                if temp_final_etc_overal != 'SELL':
                                                    final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'SELL'
                                                    temp_final_etc_overal = 'SELL'
                                                    priceclose = close[i]
                                            else:
                                                candel_counter = i+6
                                                priceclosetemp = close[i]
                                                
                                        else:
                                            candel_counter = i+6
                                            priceclosetemp = close[i]

                                    else:
                                        if (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] ==  'GOOD TREND' or data2.loc[i,'TREND POWER'+'-'+self.timefrTR] =='GREAT TREND'):
                                            if (data2.loc[i,'TREND'+'-'+self.timefrTR] == 'UPTREND') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'BUY  1') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'BUY  2') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'BUY  3') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'BUY  4') :
                                                #if ((data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  2') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  3') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  4')):
                                                    candel_counter = 0
                                            else:
                                                candel_counter = i+6
                                                priceclosetemp = close[i]
                                        else:
                                            candel_counter = i+6
                                            priceclosetemp = close[i]


                                elif final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] == 'BUY':
                                        if (data2.loc[i,'TREND'+'-'+self.timefrTR] == 'UPTREND') :
                                            if ((data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'BUY  2') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'BUY  3') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'BUY  4')):
                                                ##print(data2.loc[i,'TREND POWER'+'-'+self.timefrTR])
                                                if ((data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == 'GOOD TREND') or (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == 'GREAT TREND') or (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] == 'WEAK TREND')):
                                                    if temp_final_etc_overal != 'BUY':
                                                        final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'BUY'
                                                        temp_final_etc_overal = 'BUY'
                                                        priceclose = close[i]
                                                else:
                                                    candel_counter = i+6
                                                    priceclosetemp = close[i]
                                                    
                                            else:
                                                candel_counter = i+6
                                                priceclosetemp = close[i]

                                        else:
                                            if (data2.loc[i,'TREND POWER'+'-'+self.timefrTR] ==  'GOOD TREND' or data2.loc[i,'TREND POWER'+'-'+self.timefrTR] =='GREAT TREND'):
                                                if (data2.loc[i,'TREND'+'-'+self.timefrTR] == 'DOWNTREND') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'SELL  1') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'SELL  2') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'SELL  3') or (data2.loc[i,'DELTA'+'-'+self.timefrTR] == 'SELL  4') :
                                                    #if ((data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  2') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  3') and (data2.loc[i,'DELTA'+'-'+self.timefrTR] != 'BUY  4')):
                                                        candel_counter = 0
                                                else:
                                                    candel_counter = i+6
                                                    priceclosetemp = close[i]
                                            else:
                                                candel_counter = i+6
                                                priceclosetemp = close[i]                                       
                                
                                 
                                if candel_counter == i:
                                    if temp_final_etc == 'SELL':
                                        if priceclosetemp > close[i]:
                                            if temp_final_etc_overal != 'SELL':
                                                final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'SELL'
                                                temp_final_etc_overal = 'SELL'
                                                priceclose = close[i]
                                    elif temp_final_etc == 'BUY':
                                        if priceclosetemp < close[i]:
                                            if temp_final_etc_overal != 'BUY':
                                                final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'BUY'
                                                temp_final_etc_overal = 'BUY'
                                                priceclose = close[i]


                                    
                                else: 
                                    if temp_final_etc == 'SELL':
                                        if data2.loc[i,'TREND'+'-'+self.timefrTR] == 'DOWNTREND':
                                            if temp_final_etc_overal != 'SELL':
                                                final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'SELL'
                                                temp_final_etc_overal = 'SELL'
                                                priceclose = close[i]
                                    if temp_final_etc == 'BUY':
                                        if data2.loc[i,'TREND'+'-'+self.timefrTR] == 'UPTREND':
                                            if temp_final_etc_overal != 'BUY':
                                                final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'BUY'
                                                temp_final_etc_overal = 'BUY'
                                                priceclose = close[i]




                        


                                ## OVERAL LOSS LIMIT CALCULATION
                                if (final_signal_overal['OVERAL SIGNAL'].last_valid_index() != None) and ((final_signal_overal.loc[i,'OVERAL SIGNAL'] != 'BUY') or (final_signal_overal.loc[i,'OVERAL SIGNAL'] != 'SELL')):
                                    if final_signal_overal.loc[final_signal_overal['OVERAL SIGNAL'].last_valid_index(),'OVERAL SIGNAL'] == 'SELL':
                                        if close[i] > (1+lossindex)*priceclose:
                                            final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'STOP LIMIT, CLOSE THE SELL POSITION'
                                            
                                    if final_signal_overal.loc[final_signal_overal['OVERAL SIGNAL'].last_valid_index(),'OVERAL SIGNAL'] == 'BUY':
                                        if close[i] < (1-lossindex)*priceclose:
                                            final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'STOP LIMIT, CLOSE THE BUY POSITION'
                                            



                                

                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell

                                                               
                                if final_signal.loc[i,'MACHINE SIGNAL'] == 'SELL':
                                        price_TEMP_sell_machin = close[i]
                                        if    price_TEMP_BUY_machin != 0:
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell_machin-price_TEMP_BUY_machin
                                            if final_signal.loc[i,'REVENUE'] > 0 : 
                                                win = win+1
                                            elif  final_signal.loc[i,'REVENUE'] < 0 : loss = loss+1
                                    
                                elif final_signal.loc[i,'MACHINE SIGNAL'] == 'BUY':
                                        price_TEMP_BUY_machin = close[i] 
                                        if    price_TEMP_sell_machin != 0:  
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell_machin-price_TEMP_BUY_machin
                                            if final_signal.loc[i,'REVENUE'] > 0 : 
                                                win = win+1
                                            elif  final_signal.loc[i,'REVENUE'] < 0 : loss = loss+1

    


                                
                                if final_signal_overal.loc[i,'OVERAL SIGNAL'] == 'SELL':
                                        price_TEMP_sell = close[i]
                                        if    price_TEMP_BUY != 0:
                                            final_signal_overal.loc[i,'OVERAL REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                            if final_signal_overal.loc[i,'OVERAL REVENUE'] > 0 : 
                                                win_overal = win_overal+1
                                            elif  final_signal_overal.loc[i,'OVERAL REVENUE'] < 0 : loss_overal = loss_overal+1
                                    
                                elif final_signal_overal.loc[i,'OVERAL SIGNAL'] == 'BUY':
                                        price_TEMP_BUY = close[i] 
                                        if    price_TEMP_sell != 0:  
                                            final_signal_overal.loc[i,'OVERAL REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                            if final_signal_overal.loc[i,'OVERAL REVENUE'] > 0 : 
                                                win_overal = win_overal+1
                                            elif  final_signal_overal.loc[i,'OVERAL REVENUE'] < 0 : loss_overal = loss_overal+1


                              
                            elif ('SAF' or 'USD') in esmm:
                              
                                final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefrTR] = data2.loc[i,'FINAL SIGNAL'+'-'+self.timefrTR]
                                final_signal_overal.loc[i,'CHIKOU'+'-'+self.timefrTR] = data2.loc[i,'Chikou'+'-'+self.timefrTR]
                                final_signal_overal.loc[i,'Delta'+'-'+self.timefrTR] = data2.loc[i,'DELTA'+'-'+self.timefrTR]
                                final_signal_overal.loc[i,'Power Trend'+'-'+self.timefrTR] = data2.loc[i,'TREND POWER'+'-'+self.timefrTR]
                                final_signal_overal.loc[i,'Trend'+'-'+self.timefrTR] = data2.loc[i,'TREND'+'-'+self.timefrTR]
                              
                              
                                TEMP_SIG = 'none'

                                
                                if data2.loc[i,'STOCH-SIGNAL'] == 'BUY' : TEMP_STOCH = 'BUY'
                                if data2.loc[i,'STOCH-SIGNAL'] == 'SELL' : TEMP_STOCH = 'SELL'

                                ## FINAL SIGNAL SAFFRON
                                final_signal.loc[i,'CCI14-SIGNAL'] = data2.loc[i,'CCI14-SIGNAL']
                                final_signal.loc[i,'CCI14-SIGNAL-based on 180'] = data2.loc[i,'CCI14-SIGNAL-based on 180']          
                                
                                


                                ## CALCULATING DELTA
                                if (count_BUY - count_sell) > 0 :  final_signal.loc[i,'DELTA'] = 'BUY  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) < 0 :  final_signal.loc[i,'DELTA'] = 'SELL  '+str(abs(count_BUY-count_sell))
                                elif (count_BUY - count_sell) == 0 :  final_signal.loc[i,'DELTA'] = str(abs(count_BUY-count_sell))
                                
                                final_signal.loc[i,'TREND POWER'] = data2.loc[i,'TREND-ADX']

                                if data2.loc[i,'TREND-MACD5'] == 'UPTREND' or data2.loc[i,'TREND-MACD5'] == 'DOWNTREND':
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-MACD5']

                                if data2.loc[i,'TREND-CCI14'] == 'UPTREND' or data2.loc[i,'TREND-CCI14'] =='DOWNTREND' :
                                    final_signal.loc[i,'TREND'] = data2.loc[i,'TREND-CCI14']
                            
                                if data2.loc[i,'CCI14-SIGNAL'] == 'BUY' :
                                    TEMP_CCI = 'BUY'
                                    if (count_BUY - count_sell) > 2 : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - WITHOUT STOCH'
                                    if ((count_sell > count_BUY) and (final_signal.loc[i,'TREND'] != 'UPTREND')):final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL, Notice For BUY'
                                
                                if data2.loc[i,'CCI14-SIGNAL'] == 'SELL' :
                                    TEMP_CCI = 'SELL'
                                    if (count_sell - count_BUY) > 2 : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - WITHOUT STOCH'
                                    elif (count_sell < count_BUY) and (final_signal.loc[i,'TREND'] != 'DOWNTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL, Notice For SELL'
                                if (TEMP_CCI == 'BUY') and (count_BUY-count_sell >= 4) and (final_signal.loc[i,'TREND'] == 'UPTREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY - LAST CCI BUY'
                                if (TEMP_CCI == 'SELL') and (count_sell-count_BUY >= 4) and (final_signal.loc[i,'TREND'] == 'DOWNTREND') : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL - LAST CCI SELL'

                                if (TEMP_STOCH == 'BUY') and (TEMP_CCI == "BUY"):
                                    if ((count_BUY-count_sell >= 2) and (final_signal.loc[i,'TREND'] == 'UPTREND')) : 
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                    if (data2.loc[i,'TREND-ADX'] == 'WEAK TREND') and (final_signal.loc[i,'TREND'] != 'UPTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'ESLAH BAZAR'

                                if (TEMP_STOCH == 'SELL') and (TEMP_CCI == "SELL"):
                                    if ((count_BUY-count_sell <= 2) and (final_signal.loc[i,'TREND'] == 'DOWNTREND')) : 
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                    if (data2.loc[i,'TREND-ADX'] == 'WEAK TREND') and (final_signal.loc[i,'TREND'] != 'DOWNTREND'):
                                        final_signal.loc[i,'MACHINE SIGNAL'] = 'ESLAH BAZAR'
                                
                                if (count_sell > count_BUY) and (data2.loc[i,'STOCH-SIGNAL'] == 'Over Bought'):
                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT - STOCH OVER BOUGHT'
                                    TEMP_SIG = 'WAIT - STOCH OVER BOUGHT'
                                if (TEMP_SIG == 'WAIT - STOCH OVER BOUGHT'):
                                        if (TEMP_CCI == 'SELL') and (TEMP_STOCH == 'SELL') and (count_BUY < count_sell) and (final_signal.loc[i,'TREND POWER'] == ('WEAK TREND')): final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'
                                        if (TEMP_CCI == 'SELL') and (TEMP_STOCH == 'SELL') and (count_BUY > count_sell) : final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT '
                                    #if (TEMP_CCI == 'SELL') and (TEMP_STOCH == 'SELL') and (count_BUY == count_sell) : final_signal.loc[i,'MACHINE SIGNAL'] = 'SELL'

                                if (count_BUY > count_sell) and (data2.loc[i,'STOCH-SIGNAL'] == 'Over Sold'):
                                    final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT - STOCH OVER SOLD'
                                    TEMP_SIG = 'WAIT - STOCH OVER SOLD'
                                if (TEMP_SIG == 'WAIT - STOCH OVER SOLD'):
                                        if (TEMP_CCI == 'BUY') and (TEMP_STOCH == 'BUY') and (count_BUY > count_sell) and  (final_signal.loc[i,'TREND POWER'] == ('WEAK TREND')) : final_signal.loc[i,'MACHINE SIGNAL'] = 'BUY'
                                        if (TEMP_CCI == 'BUY') and (TEMP_STOCH == 'BUY') and (count_BUY < count_sell) : final_signal.loc[i,'MACHINE SIGNAL'] = 'WAIT '
                                

                                if (data2.loc[i,'CCI14-SIGNAL'] == 'BUY') and (final_signal.loc[i,'TREND POWER'] == ('GOOD' or 'GREAT')) and ((final_signal.loc[i,'TREND'] == 'DOWNTREND') or (final_signal.loc[i+1,'TREND'] == 'DOWNTREND')): final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL'
                                if (data2.loc[i,'CCI14-SIGNAL'] == 'SELL') and (final_signal.loc[i,'TREND POWER'] == ('GOOD' or 'GREAT')) and ((final_signal.loc[i,'TREND'] == 'UPTREND') or (final_signal.loc[i+1,'TREND'] == 'UPTREND')): final_signal.loc[i,'MACHINE SIGNAL'] = 'BE CAREFUL'    
                                
                                if  data2.loc[i,'ADX-SIGNAL'] == 'YELLOW WARNING':
                                    final_signal.loc[i,'MACHINE SIGNAL'] = "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning"
                                    
                                final_signal.loc[i,'COUNT-BUY'] = count_BUY
                                final_signal.loc[i,'COUNT- SELL'] = count_sell
                                
                                
                            


                                if ((LAST_CCI_200 == 'BUY') or (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'BUY')):


                                    if (final_signal.loc[i,'Chikou'] == 'UPTREND'):
                                        #if tempfinal != 'BUY':
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR BUY'
                                            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'NOTICE FOR BUY'
                                            
                                            #tempfinal = 'BUY'
                                    
                                    #if ((final_signal.loc[i,'MACHINE SIGNAL']=='BUY - WITHOUT STOCH' )):
                                            
                                    #            final_signal.loc[i,'FINAL SIGNAL'] = 'BUY IS AN OPTION'
                                    #            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'BUY IS AN OPTION'
                                                
                                    
                                    if (TEMP_STOCH == 'BUY'):
                                        if (final_signal.loc[i,'MACHINE SIGNAL']=='BUY - LAST CCI BUY'):
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR BUY' 
                                            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'NOTICE FOR BUY'

                                        if (((final_signal.loc[i,'MACHINE SIGNAL'] == "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning") and (count_BUY-count_sell>=3)) or (final_signal.loc[i,'MACHINE SIGNAL']=='BUY' )):
                                            if tempfinal != 'BUY':
                                                final_signal.loc[i,'FINAL SIGNAL'] = 'BUY'
                                                final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'BUY'
                                                tempfinal = 'BUY'
                                                if (data2.loc[i,'TREND'+'-'+self.timefrTR] == 'UPTREND') :
                                                    if (data2.loc[i,'DELTA'+'-'+self.timefrTR] == ( 'BUY  2'or 'BUY  3'or 'BUY  4')):
                                                        final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'BUY'
                                    
                                

                                                


                                if ((LAST_CCI_200 == 'sell') or (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'SELL')):
                                    ##print(final_signal.loc[i,'MACHINE SIGNAL'])
                                    if (final_signal.loc[i,'Chikou'] == 'DOWNTREND'):
                                       # if tempfinal != 'sell':
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR SELL'
                                            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'NOTICE FOR SELL'
                                        #    tempfinal = 'sell'
                                    #if ((final_signal.loc[i,'MACHINE SIGNAL']=='SELL - WITHOUT STOCH' )):
                                            
                                    #            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR SELL'
                                    #            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'NOTICE FOR SELL'
                                            

                                    if (TEMP_STOCH == 'SELL'):
                                        if (final_signal.loc[i,'MACHINE SIGNAL']=='SELL - LAST CCI SELL'):
                                            final_signal.loc[i,'FINAL SIGNAL'] = 'NOTICE FOR SELL' 
                                            final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'NOTICE FOR SELL' 

                                        if (((final_signal.loc[i,'MACHINE SIGNAL'] == "OOPS CHECK ADX SIGNAL, IT's YELLOW Warning") and (count_sell-count_BUY>=3)) or (final_signal.loc[i,'MACHINE SIGNAL']=='SELL' ) ):
                                            if tempfinal != 'sell':
                                                final_signal.loc[i,'FINAL SIGNAL'] = 'SELL'
                                                final_signal_overal.loc[i,'Machine Signal'+'-'+self.timefr] = 'SELL'
                                                tempfinal = 'sell'                         
                                                if data2.loc[i,'TREND'+'-'+self.timefrTR] == 'DOWNTREND':
                                                    if data2.loc[i,'DELTA'+'-'+self.timefrTR] == ( 'SELL  2'or 'SELL  3'or 'SELL  4'):
                                                        final_signal_overal.loc[i,'OVERAL SIGNAL'] = 'SELL'


                                    

                                    

                                if (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'SELL'):
                                    LAST_CCI_200 = 'sell'
                                if (final_signal.loc[i,'CCI14-SIGNAL-based on 180'] == 'BUY'):
                                    LAST_CCI_200 = 'BUY' 
                                
                                
                                ## REVENUE CALCULATING it not working properly when two sell or BUY signal come immideatly
                                if final_signal.loc[i,'FINAL SIGNAL'] == 'SELL':
                                        price_TEMP_sell = close[i]
                                        if    price_TEMP_BUY != 0:
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                            if final_signal.loc[i,'REVENUE'] > 0 : 
                                                win = win+1
                                            elif  final_signal.loc[i,'REVENUE'] < 0 : loss = loss+1
                                    
                                elif final_signal.loc[i,'FINAL SIGNAL'] == 'BUY':
                                        price_TEMP_BUY = close[i] 
                                        if    price_TEMP_sell != 0:  
                                            final_signal.loc[i,'REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                            if final_signal.loc[i,'REVENUE'] > 0 : 
                                                win = win+1
                                            elif  final_signal.loc[i,'REVENUE'] < 0 : loss = loss+1
                            

                                                                                               
                                
                                
                                if final_signal_overal.loc[i,'OVERAL SIGNAL'] == 'SELL':
                                        price_TEMP_sell = close[i]
                                        if    price_TEMP_BUY != 0:
                                            final_signal_overal.loc[i,'OVERAL REVENUE'] = price_TEMP_BUY-price_TEMP_sell
                                            if final_signal_overal.loc[i,'OVERAL REVENUE'] > 0 : 
                                                win_overal = win_overal+1
                                            elif  final_signal_overal.loc[i,'OVERAL REVENUE'] < 0 : loss_overal = loss_overal+1
                                    
                                elif final_signal_overal.loc[i,'OVERAL SIGNAL'] == 'BUY':
                                        price_TEMP_BUY = close[i] 
                                        if    price_TEMP_sell != 0:  
                                            final_signal_overal.loc[i,'OVERAL REVENUE'] = price_TEMP_sell-price_TEMP_BUY
                                            if final_signal_overal.loc[i,'OVERAL REVENUE'] > 0 : 
                                                win_overal = win_overal+1
                                            elif  final_signal_overal.loc[i,'OVERAL REVENUE'] < 0 : loss_overal = loss_overal+1


                        

                        if (loss+win) != 0:
                            final_signal.loc[i,'WinRate'] = (win/(loss+win))*100
                        if ((loss_overal+win_overal)) != 0:
                            final_signal_overal.loc[i,'WINRATE'] = (win_overal/(loss_overal+win_overal))*100
                        final_signal['STOCHSIGNAL'] = data2['STOCH-SIGNAL']
                        
                        final_signal_print = final_signal.add_suffix('-'+self.timefr)
                        final_signal_print.loc[i,'REVENUE'+'-'+self.timefr] =  final_signal_print['REVENUE'+'-'+self.timefr].sum()
                        final_signal_overal.loc[i,'OVERAL REVENUE'] =  final_signal_overal['OVERAL REVENUE'].sum()
                        del  final_signal_print['COUNT-BUY'+'-'+self.timefr]
                        del  final_signal_print['COUNT- SELL'+'-'+self.timefr]
                        del  final_signal_print['CCI14-SIGNAL'+'-'+self.timefr]
                        final_signal_print.dropna(how='all', axis=1, inplace=True)
                        
                        return data2,final_signal_print,final_signal_overal

        def connect(self):

                username = 2771749
                server1 = "MofidSecurities-Server"

                                                # establish MetaTrader 5 connection to a specified trading account
                if not mt5.initialize(login=2771749, server="MofidSecurities-Server" ,password="vubrbdBySk94Qpa*"):
                    ##print("initialize() failed, error code =",mt5.last_error())
                    quit()
                    
        def cal_TREND(self,hour,close,high,low,openn,esmm,vol): 
        
            rsi = pd.DataFrame(talib.RSI(close,14))
            ###print("\n\n\n\n RSI NUMPY ",rsi.iloc[:,0],"\n\n\n\n\n\n\n\n close",close, type(close),type(rsi))
            mfi = pd.DataFrame(talib.MFI(high, low, close, vol, 14))
            mfi.rename(columns={0:"MFI"},inplace=True)
            macd = pd.DataFrame(talib.MACD(close,12,26,9 ))
            macd = macd.T
            macd.rename(columns={0:"macd",1:"signal-macd",2:'Histogram-macd'},inplace=True)
            
            macd5 = pd.DataFrame(talib.MACD(close,5,35,5 ))
            macd5 = macd5.T
            macd5.rename(columns={0:"macd5",1:"signal-macd5",2:'Histogram-macd5'},inplace=True)
            
            macdfx = pd.DataFrame(talib.MACDFIX(close,14))
            macdfx = macdfx.T
            macdfx.rename(columns={0:"macdfx",1:"signal-macdfx",2:'Histogram-macdfx'},inplace=True)
            
            dema = pd.DataFrame(talib.DEMA(close,timeperiod=14))
            dema.rename(columns={0:"Dema"},inplace=True)
            stochrsi = self.STOCH(rsi,14,3)

            cci14 = pd.DataFrame(talib.CCI(high, low, close, timeperiod=14))

            natr = pd.DataFrame(talib.NATR(high, low, close, timeperiod=14))
            
            adx = pd.DataFrame(talib.ADX(high, low, close, timeperiod=14)) 
            
            plusdi = pd.DataFrame(talib.PLUS_DI(high, low,close, timeperiod=14)) 
            
            mindi = pd.DataFrame(talib.MINUS_DI(high, low,close, timeperiod=14)) 
            finaldata= pd.concat([rsi,stochrsi,cci14,macd,macd5,macdfx,adx,plusdi,mindi,dema,mfi], axis=1)
            finaldata.columns=['RSI','STOCHRSI-K-Fast','STOCHRSI-D-Fast','STOCHRSI-K-SLOW','STOCHRSI-D-SLOW','CCI14','MACD','signal-macd','Histogram-macd','MACD5','signal-macd5','Histogram-macd5','MACDFX','signal-macdfx','Histogram-macdfx','ADX','PLUS DI','MINUS DI','DEMA','MFI']
            finaldata['hour'] = hour
            finaldata2 = finaldata.copy()
            finaldata2 , finaldata3 = self.signal_TREND(finaldata2,close,openn,esmm)
            ###print(finaldata3)
            #finaldata2 = finaldata2[::-1]
            #finaldata3 = finaldata3[::-1]
            #finaldata = finaldata[::-1]
            
            return finaldata,finaldata2,finaldata3
        def cal(self,hour,close,high,low,openn,esmm,vol,trend): 
        
            rsi = pd.DataFrame(talib.RSI(close,14))
            
            mfi = pd.DataFrame(talib.MFI(high, low, close, vol, 14))
            mfi.rename(columns={0:"MFI"},inplace=True)
            macd = pd.DataFrame(talib.MACD(close,12,26,9 ))
            macd = macd.T
            macd.rename(columns={0:"macd",1:"signal-macd",2:'Histogram-macd'},inplace=True)
            
            macd5 = pd.DataFrame(talib.MACD(close,5,35,5 ))
            macd5 = macd5.T
            macd5.rename(columns={0:"macd5",1:"signal-macd5",2:'Histogram-macd5'},inplace=True)
            
            macdfx = pd.DataFrame(talib.MACDFIX(close,14))
            macdfx = macdfx.T
            macdfx.rename(columns={0:"macdfx",1:"signal-macdfx",2:'Histogram-macdfx'},inplace=True)
            
            dema = pd.DataFrame(talib.DEMA(close,timeperiod=14))
            dema.rename(columns={0:"Dema"},inplace=True)
            stochrsi = self.STOCH(rsi,14,3)

            cci14 = pd.DataFrame(talib.CCI(high, low, close, timeperiod=14))

            natr = pd.DataFrame(talib.NATR(high, low, close, timeperiod=14))
            
            adx = pd.DataFrame(talib.ADX(high, low, close, timeperiod=14)) 
            
            plusdi = pd.DataFrame(talib.PLUS_DI(high, low,close, timeperiod=14)) 
            
            mindi = pd.DataFrame(talib.MINUS_DI(high, low,close, timeperiod=14)) 
            finaldata= pd.concat([rsi,stochrsi,cci14,macd,macd5,macdfx,adx,plusdi,mindi,dema,mfi], axis=1)
            finaldata.columns=['RSI','STOCHRSI-K-Fast','STOCHRSI-D-Fast','STOCHRSI-K-SLOW','STOCHRSI-D-SLOW','CCI14','MACD','signal-macd','Histogram-macd','MACD5','signal-macd5','Histogram-macd5','MACDFX','signal-macdfx','Histogram-macdfx','ADX','PLUS DI','MINUS DI','DEMA','MFI']
            finaldata['hour'] = hour
            finaldata2 = finaldata.copy()
            
            
            finaldata2 , finaldata3,finaldata4 = self.signal(finaldata2,close,openn,esmm,trend)
            ###print(finaldata3)
            finaldata2 = finaldata2[::-1]
            finaldata3 = finaldata3[::-1]
            finaldata = finaldata[::-1]
            
            return finaldata,finaldata2,finaldata3,finaldata4
        def STOCH(self,rsi,lenght_rsi,smooth_d):
            lenght_rsi = lenght_rsi-1
            kslow = np.empty([rsi.size])
            Dslow = np.empty([rsi.size])
            Dfast = np.empty([rsi.size])
            for i in range(lenght_rsi,len(rsi)):
                kslow[i] = ((rsi.loc[i,0] - min(rsi.loc[i-lenght_rsi:i,0]))/(max(rsi.loc[i-lenght_rsi:i,0]-min(rsi.loc[i-lenght_rsi:i,0]))))*100
                Dslow[i] = (kslow[i]+kslow[i-1]+kslow[i-2])/3
                Dfast[i] = (Dslow[i]+Dslow[i-1]+Dslow[i-2])/3
            
            Kslow = pd.DataFrame(kslow, columns = ['k-slow'])
            dslow = pd.DataFrame(Dslow, columns = ['D-slow'])
            kfast = pd.DataFrame(Dslow, columns = ['K-fast'])
            dfast = pd.DataFrame(Dfast, columns = ['D-fast'])
            stoch = pd.concat([Kslow,dslow,kfast,dfast], axis=1)
            return stoch
        def pandaaETH(self,the_array):
            array = np.empty([the_array.size,6])
            for i in range(the_array.size):
                for j in range(6):
                    array[i,j] = the_array[i][j]
            
            
            #array = np.delete(array,0,1)
            return  array              
        def pandaa(self,the_array):
            array = np.empty([the_array.size,8])
            for i in range(the_array.size):
                for j in range(8):
                    array[i,j] = the_array[i][j]
            
            
            #array = np.delete(array,0,1)
            return  array    



    
app = QApplication(sys.argv)
MainWindow = QMainWindow()
ui = Ui_MainWindow()
ui.setupUi(MainWindow)
MainWindow.show()
sys.exit(app.exec_())
