@echo off
title yt-dlp M4A Downloader


echo ==============================
echo   YouTube to M4A Downloader
echo ==============================
echo.
set /p URL=Paste video URL and press ENTER:
echo.

yt-dlp -f bestaudio[ext=m4a] --embed-thumbnail --add-metadata "%URL%"

echo.
echo Download finished.
pause
