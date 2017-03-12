all:	../SOCKIT_DRV.exe ../SOCKIT_D64.exe

../SOCKIT_DRV.exe:	SOCKIT_DRV.7z
	cat 7zSD.sfx config.txt SOCKIT_DRV.7z > ../SOCKIT_DRV.exe

../SOCKIT_D64.exe:	SOCKIT_D64.7z
	cat 7zSD.sfx config.txt SOCKIT_D64.7z > ../SOCKIT_D64.exe

SOCKIT_DRV.7z:
	cd files && 7za a ../$@ *
	cd dpinst && 7za a ../$@ dpinst.exe

SOCKIT_D64.7z:
	cd files && 7za a ../$@ *
	cd dpinst64 && 7za a ../$@ dpinst.exe

clean:
	rm SOCKIT_DRV.7z SOCKIT_D64.7z
