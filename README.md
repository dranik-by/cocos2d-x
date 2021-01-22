# Cocos2d-x
Install Cocos2d-x for Linux

# Fix lib chipmunk
https://github.com/cocos2d/cocos2d-x/issues/20471

# Copy libchipmunk.a
libchipmunk7.0.1/libchipmunk.a cocos2d-x/external/chipmunk/prebuilt/linux/64-bit/libchipmunk.a

# Code
create Scene:
    cocos2d::Director::getInstance()->pushScene(cocos2d::TransitionFade::create(0.5f, NameScene::createScene()));

remove Scene:
    cocos2d::Director::getInstance()->popScene(cocos2d::TransitionFade::create(0.5f, NameScene::removeScene()));
