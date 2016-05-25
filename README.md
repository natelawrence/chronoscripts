# chronoscripts
Frankly, at this point, I'm just looking for a user-friendly version control reporting system for transcription and subtitling.

At present I have several different formattings of each transcript and it is difficult to consistently update each of them as corrections to transcription is made. 

Ultimately, I wish to create a workflow and toolset for creating perfect textual transcriptions of what is spoken in a piece of audio or video.

This is desirable for purposes of accuracy and representing to the hearing impaired exactly what the speaker has spoken, exactly as they have spoken it.

Once this level of precision has been achieved, it is possible to perform forced alignment of the text to the audio, which inherently makes the audio searchable. See Lower Quality's 'Gentle' for an easy to use forced aligner.

I wish to have such precision in the alignment that each alphanumeric character (and spaces) in a transcript is able to act as a hyperlink to the media player's progress bar.

Once this timing information is created, animation of the text is possible, in time with when it is heard in the audio.

This allows you to make each character visible as it is heard, creating the illusion of the speaker speaking the text into existence.

The text may be presented in article/interview format arranged in paragraphs, presented in the format of subtitles or closed captions, or scrolled through in the style of a ticker tape (or combinations of these presentations).

Once a transcript is found to be truly flawlessly verbatim, it should be possible to proofread it to remove "um"s, "uh"s, repeated words when forming thoughts, correct mispronunciations, etc. and still retain the timing information for the remaining words. 

For that matter, if that information is tied back to either an audio editor or media player, it would be possible to skip, mute, delete, or fold out of view the portions of audio which correspond to those edited out repeated words, stutters, etc. 

Ideally the difference between verbatim and proofread is merely markup within the same file, as are the beginning and ending of words, sentences, caption block line breaks, and paragraphs - all able to be independently toggled at any point.

If a subtitle format already exists which allows the storage of a single copy of each word in a transcript and allows time codes for each character's appearance, I am not yet aware of it, however it should be possible, once time codes are created, to (in standard subtitle and caption formats) create as many iterations of a block of captions as there are characters within it, in order to enable per-character printing of the subtitle to screen as the words are spoken. This is a bit of a hack of existing subtitle formats and not good for interactive transcripts generated from the subtitles/captions, but to the typical viewer should look correct as subtitles (again, to translators, not so much). 

Characters within a caption block which have not yet been drawn should have space character placeholders. It may also prove desirable to pad the beginning and end of the shorter of two lines in a block of captions with spaces so that the two lines appear the same width if the user's subtitle/caption settings are using background visible, rather than window visible.

In the process of transcription, alignment, homophone substitution or vocabulary expansion, transcript review, manually creating time codes for words which the forced aligner failed to match, deciding where line breaks ought to occur in converting each sentence to caption blocks, and updating caption block timing with the begin and end time codes for the first and last words in that block of captions, it will be desirable to be able to tag specific words as inserted by the editor when they are implied by the original author but not explicitely heard in the audio, tag portions of transcription as in doubt or list multiple possible transcriptions for a short difficult to hear portion of audio, have verbatim and proofread copies of certain words (think "kinda'" vs. "kind of" or "Pacifically" vs. "specifically"),  etc. 

Once per-word start and end time codes are created and used to create caption block start and end time codes, every caption block's end/off time should be extended to the beginning of the next block of captions until the sentence ends. Captions disappearing between words in the same sentence is very disruptive to reading along, unless there is a significant pause/silence in the middle of a sentence. Disappearance of the caption block between sentences is acceptable and even desirable, so long as there is a typical pause between them.

Punctuation between words ought generally to appear within the time that the letter which that punctuation is directly adjacent to has to appear. If there is any space between the words in the audio, then that time duration may be divided by the number of characters which are not directly adjacent to a letter or numeral (for example a hyphen surrounded by two spaces or an ellipsis represented by individual periods, rather than a single ellipsis character between words)

I intend for this overview to be cleaned up at a later date, but this is a sketch of many of the primary ideas. 
For the time being, however, this will simply be a repository of different versions of transcripts.
