# Contact reminders for power connectors

This repo contains an Excel workbook (built with Excel for Mac 2019) to
accomplish the core bookkeeping in [How to be a Power
Connector](https://isbnsearch.org/isbn/9780071830737) by Judy Robinett.

Robinett argues that the heart of "networking" or "strategic relationship
management" is the following workflow:

- Identify your "tribe" of relationships encompassing all of your life,
  business and personal. Its size will roughly be [Dunbar's
  number](https://en.wikipedia.org/wiki/Dunbar%27s_number) (100-250, nominally
  ~150).
- Divide that "tribe" into a few "power circles" or frequency tiers (Robinett
  suggests three tiers: 5 + 50 + 100 = 155).
- Commit to a frequency of contact for each power circle (Robinett suggests
  being in touch with each of the 5 daily, each of the 50 weekly, and each of
  the 100 monthly) and reach out to add value to these people at least this
  often.
- Continually upgrade these power circles as you meet worthwhile new people and
  others inevitably roll off the bottom.

This workbook provides a place to maintain a list of people, their place in
one's power circles, and information about the most recent contact for each of
them. It uses some conditional formatting and custom sorting to make it
comfortable to carry out Robinett's proposal in practice, reviewing at a glance
when "it has been too long" with someone.

Robinett's recommendations add up to a baseline of adding value to ~15
different people in one's power circles every day, 365 days a year. I don't
consider this realistic for people with an occupation other than "full-time
networker."

This spreadsheet's defaults for the sizes and frequencies of the tiers dial
these parameters down a great deal while staying true to Robinett's basic
Dunbar's-number-based structure:

- The default power circle sizes are 5 + 25 + 120 = 150.
- The spreadsheet suggests being in touch with each of the 5 weekly, each of
  the 25 every 4 weeks, and each of the 120 every 16 weeks. This adds up to a
  few people every day. (5/7 + 25/28 + 120/112 = 2.68, but the number of people
  you contact on an average day will be higher, as you will often connect with
  people spontaneously before they've fallen to 0% recency in the spreadsheet.)

I've found this intensity to be sustainable in lieu of being on social media.
It consumes similar or slightly more bandwidth as, e.g., routine Facebook use,
but the relationship value enjoyed is far richer.  It helps me in my consulting
practice to keep my profesisonal network warm even when busy (e.g., when deep
in a client project).

## Initial setup

1. In place of the fake data in the `power_circles` sheet, under the columns
   `first_name`, `last_name`, `last_contacted`, and `description`, assemble a
   list of all the people you've been in touch with in the recent past and when
   and how you were in contact with them. I wrote some little scripts
   (unpublished) to merge names from social media data exports, cell phone
   contacts, etc., but in all cases, this is backbreaking given how many ways
   (including analog in-person interactions) one connects with people. I ended
   up with 1300-1400 people; the latter two fields were unknown for most of
   them.
1. Assign `0` to `tier` for all of these people.
1. Make a pass through all of these people. When you see a relationship that
   feels warm (or that deserves effort to get to warm), assign them an
   appropriate tier (1, 2, or 3, 3 being closest) depending on how close they
   are.
1. Use Excel's "custom sort" to sort people by tier, then by last contacted,
   then by last name. This custom sort has been saved in this spreadsheet. You
   can pull it up using `Ctrl-Shift-R` (`Cmd-Shift-R` on a Mac). You'll use
   this custom sort all of the time in this spreadsheet.
1. Massage these tier labels until their sizes are reasonably in line with the
   above guidance. They don't have to be exact (in fact my power circles are
   closer to 5 + 25 + 160 = 190).
1. Set up the maximum days between contacts you'd like to commit to for these
   tiers, and enter them in the `tiers` sheet.
1. You'll probably find that you're in the red at first with a lot of people
   below your top 50 or so. I found getting current with everyone in my power
   circles took me a couple months of pretty heavy initial outreach effort.

## Maintenance of your power circles

1. Every day, enter the date and description of your contacts with people in
   your power circles. The `Ctrl-;` shortcut key for today's date is key here.
1. Use the custom sort `Ctrl-Shift-R` (`Cmd-Shift-R`) to easily review who is
   almost overdue and overdue in your power circles.
1. Use the `average_recency` sheet to monitor how you're keeping up your
   relationship management in general. I find, between people who fall all the
   way to near-zero recency and others whom I contact more regularly and
   spontaneously, that my average recency hovers in the 57-61% range. You'll
   find in practice that this score fluctuates as you get busier and less busy
   with billable work, life events, etc.
1. Promote and demote people as they become relevant, disappear from your life,
   etc., by adding rows or adjusting their tier labels.
