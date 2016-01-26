TARGET=___FILEBASENAMEASIDENTIFIER___

all:
	# Content.swift is main.swift in Package
	[ -f main.swift ] && rm main.swift

	# -v '^import\|^//\|^[ ]*$': will match with actual codes
	[ $(grep -c -v '^import\|^//\|^[ ]*$') -ne 0 ] && cp Contents.swift main.swift 
	
	swift build

install:
    cp .build/debug/$(TARGET) .