---
layout: post
title:      "Rails Project"
date:       2020-12-18 04:35:35 +0000
permalink:  rails_project
---


For my Rails project I created a web app that will reserve a soccer Field for an Event. The Event has Requirements like goals size, food trucks, etc. I got the idea from a real world problem I encountered while in the Rails Section. 

This project presented several learning oppourtunites. The most difficult was how to block off time slots for created Events so new Events could not overlap with them. All this had to be done before adding the new Event to the table. I created a scope method that pulled all Fields with a matching name to the Event Field beign created, then check the params in the Field section of the form vs the Events tables where the ids matched the event_ids with the matching Field names. After much trial and error I got it to work!

Eventually I would like to add a payment system to the app and a way to add Users to Teams and track or limit the numbers of Events per Team.

Looking back this was a fun project and a great learning expierence.
