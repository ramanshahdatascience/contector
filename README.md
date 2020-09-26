# contector: Contact reminders for "power connectors"

In [How to be a Power Connector](https://isbnsearch.org/isbn/9780071830737),
Judy Robinett argues that the heart of "networking" or "strategic relationship
management" is the following workflow:

- Identify your "tribe" of relationships of size Dunbar's number (100-250,
  nominally ~150).
- Divide that "tribe" into a few "power circles" or quality-of-service tiers
  (Robinett suggests three tiers: 5 + 50 + 150 = 155).
- Commit to a frequency of contact for each tier (Robinett suggests being in
  touch with each of the 5 daily, each of the 50 weekly, and each of the 100
  monthly) and add value to these people at least this often.
- Continually upgrade these power circles as you meet influential new people
  and as people inevitably roll off the bottom.

This repo contains an Excel spreadsheet (built with Excel for Mac 2019) to
accomplish the bookkeeping in this workflow. It provides a place for its user
to maintain a list of these people and last-contacted dates. It uses some
conditional formatting and custom sorting to make it comfortable to carry out
Robinett's proposal in your own life.

This spreadsheet's defaults for the sizes and frequencies of the tiers are much
less aggressive than Robinett's, which I don't consider realistic for anyone
but a full-time networker. Robinett's recommendations add up to a baseline of
communicating with ~15 different people every day, 365 days a year. The default
power circle sizes are 5 + 25 + 120 = 150. The spreadsheet suggests being in
touch with each of the 5 weekly, each of the 25 every 4 weeks, and each of the
120 every 16 weeks. This adds up to between 2 and 3 different people every day.
I've found this intensity to be sustainable in lieu of being on social media.

## Initial setup

1. In place of the fake data in the `power_circles` sheet, under the columns
   `first_name`, `last_name`, `last_contacted`, and `description`, assemble a
   list of all the people you've been in touch with in the recent past and when
   and how you were in contact with them. I wrote some little scripts to merge
   names from social media data exports, cell phone contacts, etc., but in all
   cases, this is backbreaking given how many ways (including analog in-person
   meetups) one connects with people. I ended up with 1300-1400 people; the
   latter two fields were unknown for most of them.
1. Assign `0` to `tier` for all of these people.
1. Make a pass through all of these people. When you see one who be in your
   power circles, increase their tier.
1. Use Excel's "custom sort" to sort people by tier, then by last contacted,
   then by last name. This custom sort has been saved in this spreadsheet. You
   can get to it using `Ctrl-Shift-R` (`Apple-Shift-R` on a Mac). You'll use
   this custom sort all of the time in this spreadsheet.
1. Massage these tier labels until their sizes are reasonably in line with the
   above guidance. They don't have to be exact (in fact my power circles are
   closer to 5 + 25 + 170 = 200).
1. Set up the frequency of contact you'd like to commit to for these tiers, and
   enter them in the `tiers` sheet.
1. You'll probably find that you're in the red at first with a lot of people
   below your top 50 or so. I found getting to where nobody in that ~170-person
   tier was red took me a couple months of pretty heavy outreach effort.

## Maintenance of your power circles

1. Every day, enter the date and description of your contacts with people in
   your power circles.
1. Use the custom sort `Ctrl-Shift-R/Apple-Shift-R` to easily review who is
   almost overdue and overdue in your power circles.
1. Use the `average_recency` score to see how you're doing with keeping up with
   people in general. If you're steady at keeping up with them, it will hover
   around 50%. You'll find in practice that this score fluctuates as you get
   busier and less busy with billable work, life events, etc.
1. Promote and demote people as they become relevant, disappear from your life,
   etc., by adjusting their tier labels.
