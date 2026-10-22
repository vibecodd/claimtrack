Claims Journey:
 1)User Submit Claim CLM-0042 -> 2) Under Review -> 3) Accepted/Rejected(with reason) -> 4) paid(if accepted) -> 5) notify the user in both cases.

Code Journey
  Laptop -> feature branch -> pr/CI -> main merge -> Build image once -> Deploy to Staging ->  deploy the image that is tested -> Observe and rollback if needed.

journey 2 for “claims above $10,000 need a second adjuster”
  laptop -> feature branch (isolated env / unit tests) -> pr/CI (code review / security bugs) -> main -> image -> deploy to staging(Integration problems / config issues / smoke tests) -> production -> rollback if needed


