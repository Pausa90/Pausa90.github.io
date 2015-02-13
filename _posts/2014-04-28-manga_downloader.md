---
layout: post
title: Manga Downloader
categories: [personal]
tags: [java, manga, tool]
fullview: true
icon: fa fa-book fa-lg
source: Pausa90/MangaDownloader
---

MangaDownlader is a simple Java automatic tool to download manga from [MangaEden].

The project resulted from the need to download a lot of mangas and it was a Java experiment with:
<ul> 
	<li>Multithreading programming</li>
	<li>Swing GUI library</li>
	<li>HTML parsing with [jsoup] library</li>
</ul>

## Functionality

MangaDownloader can download an entire manga or resume a previously download. It is helpfull when the manga is not over and a new chapter is released.

Every manga is stored in a foldier in your file system, which is divided into many foldiers as there are chapters (each chapter is downloaded in multithreading).

Also Ubuntu user can use a bash scripts, located in extractPdfFromJPGs, to extract a pdf from the downloaded images. 

<div class="row">
	<div class="col-sm-5">
		<h4 style="text-align: center">Home</h4>
		<img src="{{ site.BASE_PATH }}/assets/images/mangaDownloader/home.png"/>
	</div>
	<div class="col-sm-7">
		<h4 style="text-align: center">Download</h4>
		<img src="{{ site.BASE_PATH }}/assets/images/mangaDownloader/download.png"/>
	</div>
</div>

<br/>

## How to Use it

To use it just follow the instructions.

#### Download the Manga

* Go to [MangaEden] and select a manga from the list (you have to find a page similar to [this one]). When you find it, just copy the url.
* Run mangaedenDownloader.jar on your system 
* Select "Full Download" or "Resume Download", according to the needs, and complete the fields as request.
* Press "Start" and wait until it has finished.

#### PDF Extraction

These project contains two scripts: "extractPdf.sh" and "mangaToPDF.sh".

To get the pdf, put the first one in the foldier where are contained chapters' directory and run the script.

The second one is a launcher and need if you want to extract more pdf "togheter". 

## Bug Notes

There is a known GUI's bug: it may happen that the update bars do not follow the download. Your download will be ok.







[MangaEden]: http://www.mangaeden.com/
[jsoup]: http://jsoup.org/
[this one]: http://www.mangaeden.com/en-manga/naruto/