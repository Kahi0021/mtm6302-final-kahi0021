
# Communication Log: Café Collector

This document records communication with the client, the clarifications received, and the decisions made during the planning of Café Collector. Private messages and personal contact details are not reproduced.

## First Contact

**Date:** November 23, 2026  
**Time sent:** 5:21 PM (verify against your email)  
**Client response:** 6:06 PM  
**Method:** Email

### Question 1: Coffee type selection
- **Question:** When users select multiple coffee types, should cafés match any or all selected types?
- **Client response:** The client preferred cafés that specialize in the selected coffee types.
- **Decision:** Use ANY-match filtering (A1).
- **Reason:** A café can appear if it specializes in at least one selected drink.

### Question 2: Café data
- **Question:** Who will provide the café data, and how many cafés are needed?
- **Client response:** The client provided five coffee types and requested approximately 10–12 local cafés.
- **Decision:** Use a fixed list of 11 cafés and five coffee types (A4).
- **Reason:** The application does not require an external API.

### Question 3: Price and popularity
- **Question:** Should price and popularity filters be included?
- **Client response:** The client confirmed that both filters should be included.
- **Decision:** Add price and popularity filters (F5).
- **Reason:** These filters help users compare cafés.

### Question 4: Like, Save, and notes
- **Question:** Should Like and Favourite be separate? Should notes be editable or deletable?
- **Client response:** The client requested that Favourite be renamed Save and that notes could be edited and deleted.
- **Decision:** Keep Like and Save as separate features. Allow users to add and remove notes. The Edit option was later excluded following instructor feedback.
- **Reason:** Like and Save have different purposes, and the interface follows the instructor's direction.

### Question 5: Clear Saved
- **Question:** Should there be a Clear Saved button?
- **Client response:** The client confirmed that this would be useful.
- **Decision:** Include a Clear Saved button (A3). It removes saved cafés only.
- **Reason:** Likes and notes should remain unchanged.

### Question 6: Error messages
- **Question:** Should the application include error messages?
- **Client response:** The client agreed that error handling would be a good idea.
- **Decision:** Include relevant validation and error messages (A6).
- **Reason:** Users should receive feedback when an action cannot be completed.


## Second Contact

**Date:** November 24, 2026  
**Time sent:** 6:20 PM  
**Client response:** 6:23 PM  
**Method:** Email

**Purpose:** Follow up to confirm the coffee-type selection, price and popularity filters, and saved-café behaviour.

### Question 1: Multiple coffee types
- **Question:** How should multiple selected coffee types work?
- **Client response:** The client confirmed that cafés specializing in either selected drink are acceptable, if time permits.
- **Decision:** Keep ANY-match filtering as an optional implementation priority.
- **Reason:** This follows the client's preference while allowing the feature to be prioritized according to available time.

### Question 2: Price and popularity filters
- **Question:** Are the price and popularity filters acceptable?
- **Client response:** The client confirmed that they work for her.
- **Decision:** Include price levels ($, $$, $$$) and popularity ratings from 1 to 5.
- **Reason:** These filters were approved by the client.

### Question 3: Clear Saved behaviour
- **Question:** What should Clear Saved remove?
- **Client response:** The client clarified that only saved cafés should be removed.
- **Decision:** Clear Saved removes saved cafés but keeps Likes and notes.
- **Reason:** Other user data should not be affected.


## Additional Development Decision

Following instructor feedback, the Edit option was removed from the planned interface. Users can add and remove notes, but cannot edit an existing note.

## Summary of Decisions

- Use five coffee types: Latte, Cappuccino, Macchiato, Americano, and Espresso.
- Include the 11 cafés provided by the client.
- Use ANY-match filtering for multiple selected coffee types if time permits.
- Include price and popularity filters.
- Keep Like and Save as separate actions.
- Allow users to add and remove notes.
- Do not include an Edit option for notes.
- Include a Saved view and Clear Saved button.
- Clear Saved removes saved cafés only; Likes and notes remain unchanged.
- Include appropriate empty-state and validation messages.


