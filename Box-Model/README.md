# CSS BOX MODEL

## PADDING:
To increase the size of the box. It happens around the content. Most of the time buttons are styled using padding so that the background is wider than the text of button.

## BORDER:
Adds border around the padding.

## MARGIN:
To separate two different items and give space between items. Margins collapses, and the largest value is selected. For example, If we set 60px & 70px margin on 2 items instead of 130px there will be a gap of 70px between them.


## box-sizing : content-box;
 Content-box is the default value of box sizing. it adds the padding and border to the main content thus making the content box larger.
Total width = content-box_width(160px) + padding(2 x 20) + border( 2 x 8) = 216px
 Total width = content-box_height(80px) + padding(2 x 20) + border( 2 x 8) = 136px

## box-sizing : border-box;
Border-box substracs the padding and border to the main content. This  makes the total width and height identical to the original content box, but cuts down the width and height of the main content.
Final width of content = content-box_width(160px) - padding(2 x 20) - border( 2 x 8) = 104px
 Final height of content = content-box_height(80px) - padding(2 x 20) - border( 2 x 8) =24px
