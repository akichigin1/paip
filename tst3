*** Settings ***
Library    SeleniumLibrary
Test Setup    Precondition: Open Browser


*** Variables ***
${SiTE_URL}    https://gas.apps.test.devsun.ru/shell/paip/main/elections/01332804-1e22-4944-aab4-807f681360ce/election_general?districtName=Единый%20пропорциональный
${BROWSER}    Chrome
${LOGIN}    02S000_user1
${PASSWORD}    AxfzhYEj5B1LDzr
${VHOD}    //*[@id="app"]/div/div/main/div/div[2]/div/div/div/div/div[6]/form/input[4]
${KIK}    //app-election-base//div[4]/div/div/div
${POLE_LOGIN}    //*[@id="app"]/div/div/main/div/div[2]/div/div/div/div/div[3]/div/div[2]/input
${POLE_PAROL}    //*[@id="app"]/div/div/main/div/div[2]/div/div/div/div/div[4]/div/div[2]/input

*** Test Cases ***
Standart login
    [Documentation]    Авторизация логин пароль
    Wait Until Element Is Visible    ${POLE_LOGIN}        
    Input Text    locator=${POLE_LOGIN}    text=${LOGIN}
    Input Password    locator=${POLE_PAROL}    password=${PASSWORD}
    Sleep    time_=3s
    Click Button    locator=${VHOD}
    Sleep    time_=7s
    Click Element    locator=${KIK}
    Sleep    time_=4s
    Click Element    locator=//app-status-toolbar-button/div/div/div
    Sleep    time_=3s
    Click Element    locator=//app-status-toolbar-button/div/app-common-modal/app-base-modal/div/div[2]/app-base-modal-default-container/div/app-base-modal-default-layout/div/div[3]/app-base-modal-default-footer/div/div/div[2]/div
    Sleep    time_=3s
    Click Element    locator=//app-election-base/gc-conditional-view-wrapper/div/g-tab-bar/div[1]/div[1]/div[7]/div/div/div
    Sleep    time_=4s
    Click Element    locator=//app-election-associations/header/g-tab-bar/div[1]/div[2]/app-election-association-table/app-base-table/div/app-base-table-header/div/div[1]/div[2]/div[1]/div/app-action-button[2]/div/span
    Sleep    time_=2s
    Click Element    locator=//app-election-association-create-modal/app-base-modal/div/div[2]/app-base-modal-default-layout/div/div[2]/app-form-generator/form/app-base-template/div/div[2]/app-base-group/div/div[2]/div/gc-async-select/app-widget-wrapper/div/div[2]/g-select/div/div/div
    Sleep    time_=2s
    Click Element    locator=//*[@id="cdk-overlay-18"]/g-select-dropdown/div/div[2]/div[1]/span
    Sleep    time_=1s
    Click Element    locator=//app-election-association-create-modal/app-base-modal/div/div[2]/app-base-modal-default-layout/div/div[3]/app-base-modal-default-footer/div/div/div[2]/div
    Sleep    time_=5s
    Click Element    locator=//app-election-association/gc-navigation-tabs/div/div/gc-navigation-tab[3]/a/div/div[1]
    Sleep    time_=2s
    Click Element    locator=//app-election-association-candidates-lists/app-candidates-list-table/app-base-table/div/app-base-table-header/div/div[1]/div[2]/div/app-action-button/div/span
    Sleep    time_=2s
    Click Element    locator=//app-election-association-candidates-lists/app-candidates-list-create-modal//g-select/div/div/div
    Sleep    time_=2s
    Click Element    locator=//*[@id="cdk-overlay-21"]/g-select-dropdown/div/div/div[1]/span
    Input Text    locator=(//app-candidates-list-create-modal//input)[1]   text=08042025
    Input Text    locator=(//app-candidates-list-create-modal//input)[2]    text=58
    Input Text    locator=(//app-candidates-list-create-modal//input)[3]    text=Кичигин.А.С.
    Input Text    locator=(//app-candidates-list-create-modal//input)[4]    text=Председатель
    Click Element    locator=//div[contains(@class, '_primary') and contains(@class, 'c_primary') and @gasbutton="primary"]/div[text()="Добавить"]
    Sleep    time_=20s
    Click Element    locator=//div[@class="navigation-tab__content" and text()=" Региональные группы "]
    Sleep    time_=2s
    Click Element    locator=//*[@id="cdk-drop-list-6"]/tr[1]/td[5]/div/div/gas-icon
    Click Element    locator=//*[@id="cdk-overlay-28"]/app-federal-candidates-list-regional-groups-table-actions/div/gas-card/div[2]/gas-vertical-menu/div/div/div/div[1]/span
    Sleep    time_=2s
    Click Element    locator=//span[@class="action-button__label" and text()=" Добавить "]
    Sleep    time_=1s
    Input Text    locator=(//gc-candidate-create-modal//input)[1]    text=Кичигин     
    Input Text    locator=(//gc-candidate-create-modal//input)[2]    text=Артем 
    Input Text    locator=(//gc-candidate-create-modal//input)[3]    text=Сергеевич 
    Input Text    locator=(//gc-candidate-create-modal//input)[4]    text=28051998
    Input Text    locator=(//gc-candidate-create-modal//input)[5]    text=1313 
    Input Text    locator=(//gc-candidate-create-modal//input)[6]    text=131313
    Input Text    locator=(//gc-candidate-create-modal//input)[7]    text=1
    Sleep    time_=3s
    Click Element    locator=//div[@class="gas-button" and text()=" Создать "]
    Sleep    time_=5S
    Click Element    locator=//div[@class="gas-button" and text()=" Продолжить "]
    Sleep    time_=3S
    Click Element    locator=//div[@class="gas-button" and text()=" Подтвердить "]
    Sleep    time_=2s
    Click Element    locator=//div[contains(@class, "breadcrumbs__link") and text()=" Списки кандидатов "]
    Sleep    time_=2s
    Click Element    locator=//span[@class="action-button__label" and text()=" Добавить "]
    Sleep    time_=2s
    Click Element    locator=//div[contains(@class, "g-select__field-placeholder") and text()="Выберите значение"]
    Sleep    time_=3s
    Click Element    locator=//span[text()="Мажоритарный"]
    Input Text    locator=(//app-candidates-list-create-modal//app-date-input//input)[1]    text=08042025
    Input Text    locator=(//app-candidates-list-create-modal//app-string-input//input)[1]    text=2
    Input Text    locator=(//app-candidates-list-create-modal//app-string-input//input)[2]    text=Кичигин.А.С
    Input Text    locator=(//app-candidates-list-create-modal//app-string-input//input)[3]    text=Председатель
    Sleep    time_=4s
    Click Element    locator=//div[@class="gas-button" and text()="Добавить"]
    Sleep    time_=7s
    Click Element    locator=//span[@class="action-button__label" and text()=" Добавить "]
    Sleep    time_=2s
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[1]    text=Кичигин
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[2]    text=Артем
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[3]    text=Сергеевич
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[4]    text=1315
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[5]    text=131414
    Input Text    locator=//gc-candidate-create-modal//app-date-input//input    text=28051990
    Click Element    locator=//div[contains(@class, "g-select__field-text")]//div[text()="Выберите значение"]
    Sleep    time_=4s
    Click Element    locator=//span[@class="fg-dropdown-async-select__option ng-star-inserted" and text()="Кизильский избирательный округ №28"]
    Click Element    locator=//div[@class="gas-button" and contains(text(), "Создать")]
    Sleep    time_=1s
    Click Element    locator=//div[@class="gas-button" and text()=" Продолжить "]
    Sleep    time_=1s
    Click Element    locator=//div[@class="gas-button" and text()=" Подтвердить "]
    Sleep    time_=5s
     #Переход по хлебным крошкам к ИО
    Click Element    locator=//div[text()=" Избирательные объединения "]
    Sleep    time_=3s
    #Переход раздел кандидат
    Click Element    locator=//div[@class="g-tab-label__title" and @title="Кандидаты"]
    Sleep    time_=4s
    #нажимаем добавить самодвижа
    Click Element    locator=//span[@class="action-button__label" and text()=" Добавить "]
    #Добавляем данные самодвижа
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[1]    text=Кичигин
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[2]    text=Артем
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[3]    text=Сергеевич
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[4]    text=1315
    Input Text    locator=(//gc-candidate-create-modal//app-string-input//input)[5]    text=131414
    Input Text    locator=//gc-candidate-create-modal//app-date-input//input    text=28051990
    Sleep    time_=4s
    Click Element    locator=//div[@class="gas-button" and text()=" Создать "]
    Sleep    time_=3s
    Click Element    locator=//div[@class="gas-button" and text()=" Продолжить "]
    Sleep    time_=2s
    Click Element    locator=//div[@class="gas-button" and text()=" Подтвердить "]
    Sleep    time_=3s
    Click Element    locator=//div[text()=" Кандидаты "]
    Sleep    time_=3s
    Click Element    locator=//div[@class="g-tab-label__title" and text()="Избирательные объединения"]
    Sleep    time_=2s
    Click Element    locator=//app-election-association-table//table//tbody//tr//td[7]/div
    Sleep    time_=1s
    Click Element    locator=//span[text()=" Открыть "]
    Sleep    time_=3s
    Click Element    locator=//div[@class="navigation-tab__content" and text()=" Доверенные лица "]
    Sleep    time_=3s
    Click Element    locator=//span[@class="action-button__label" and text()=" Добавить "]
    #Ввод доверенного
    Input Text    locator=(//authorized-confidant-create-modal//gas-tab[1]//input)[1]    text=Кичигин
    Input Text    locator=(//authorized-confidant-create-modal//gas-tab[1]//input)[2]     text=Артем
    Input Text    locator=(//authorized-confidant-create-modal//gas-tab[1]//input)[3]    text=Сергеевич
    Input Text    locator=(//authorized-confidant-create-modal//gas-tab[1]//input)[4]   text=28051990
    Input Text    locator=(//authorized-confidant-create-modal//gas-tab[1]//input)[5]    text=1234
    Input Text    locator=(//authorized-confidant-create-modal//gas-tab[1]//input)[6]   text=345678
     Sleep    time_=4s
    Click Element    locator=//div[@class="gas-button" and text()=" Создать "]
    Sleep    time_=5s
    Click Element    locator=//div[@class="gas-button" and text()=" Продолжить "]
    Sleep    time_=5s
    Click Element    locator=//div[@class="gas-button" and text()=" Подтвердить "]
    Sleep    time_=3s
    Click Element    locator=//span[text()=" Действия "]
    Sleep    time_=1s
    Click Element    locator=//span[text()=" Подтвердить ввод "]
    Sleep    time_=2s
    Click Element    locator=//span[text()=" Действия "]
    Sleep    time_=1s
    Click Element    locator=//span[text()=" Зарегистрировать "]
    Sleep    time_=2s
    Click Element    locator=//div[div[text()="Выберите значение"]]
    Sleep    time_=1s
    Click Element    locator=//span[@class="fg-dropdown-async-select__option ng-star-inserted" and contains(text(), "верхняя палата законодательного")]
    Sleep    time_=2s
    Input Text    locator=(//*[@gasinputfield])[1]    text=1223
    Input Text    locator=(//*[@gasinputfield])[2]    text=080420250000
    Input Text    locator=(//*[@gasinputfield])[3]    text=тест
    Click Element    locator=//div[@class="gas-button" and text()="Применить"]
     Sleep    time_=5s
    Click Element    locator=//span[text()=" Действия "]
    Sleep    time_=2s
    Click Element    locator=//span[text()=" Отменить регистрацию "]
    Sleep    time_=2s
    Click Element    locator=(//div[div[text()="Выберите значение"]])[1]
    Sleep    time_=2s
    Click Element    locator=//span[@class="fg-dropdown-async-select__option ng-star-inserted" and text()="Верховный суд Российской Федерации"]
    Sleep    time_=2s
    Input Text    locator=(//*[@gasinputfield])[1]    text=1223
    Input Text    locator=(//*[@gasinputfield])[2]    text=08042025
    Input Text    locator=(//*[@gasinputfield])[3]    text=тест
    Sleep    time_=2s
    Click Element    locator=(//div[@class="g-select__field"])[2]
    Sleep    time_=2s
    Click Element    locator=//span[@class="fg-dropdown-async-select__option ng-star-inserted" and text()="прочие причины"]
    Sleep    time_=2s
    Click Element    locator=//div[@class="gas-button" and text()="Применить"]
    Sleep    time_=2s
     Click Element    locator=//div[text()=" Избирательные объединения "]
    Sleep    time_=4s
    Click Element    locator=//app-election-association-table//table//tbody//tr//td[7]/div
    Sleep    time_=1s
    Click Element    locator=//span[text()=" Удалить "]
    Sleep    time_=1s
    Click Element    locator=//div[@class="gas-button" and text()=" Удалить "]
    Sleep    time_=13s
    Click Element    locator=//div[@class="g-tab-label__title" and text()="Кандидаты"]
    Sleep    time_=3s
    Click Element    locator=(//div[@class="gas-button"])[10]
    Sleep    time_=3s
    Click Element    locator=//span[text()=" Удалить "]
    Sleep    time_=1s
    Click Element    locator=//div[@class="gas-button" and text()=" Удалить "]
    Sleep    time_=3s
    Click Element    locator=//div[text()=" Формирование классификатора ИК "]    
    Sleep    time_=2s
    Click Element    locator=//div[text()=" Подтвердить "]
    Sleep    time_=5s
    Close Browser
 
*** Keywords ***
Precondition: Open Browser
    [Documentation]    Открыть : Браузер на весь экран
    Open Browser    url=${SiTE_URL}     browser=${BROWSER}
    Maximize Browser Window

Postcondition: Close Browser
    [Documentation]  Закрыть браузер 
    Close Browser
