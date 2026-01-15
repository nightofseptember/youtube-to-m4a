@echo off
title yt-dlp M4A Downloader

echo ==============================
echo   YouTube to M4A Downloader
echo ==============================
echo.
echo Paste YouTube links (one per line)
echo Press CTRL+Z then ENTER when done
echo.

yt-dlp ^
-f bestaudio[ext=m4a] ^
--embed-thumbnail ^
--add-metadata ^
-o "%%(title)s - %%(artist,creator,uploader)s.%%(ext)s" ^
-a -

echo.
echo Download finished.
pause
