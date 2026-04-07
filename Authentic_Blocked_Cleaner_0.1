// ==UserScript==
// @name        Authentic Blocked Cleaner
// @namespace        http://blog.ameba.jp
// @version        0.1
// @description        制限したブログのリストから退会ブログを排除する
// @author        Ameba Blog User
// @match        https://ameblo.jp/*
// @match        https://blog.ameba.jp/block
// @icon        https://www.google.com/s2/favicons?sz=64&domain=ameba.jp
// @noframes
// @grant        none
// @updateURL        https://github.com/personwritep/Authentic_Blocked_Cleaner/raw/main/Authentic_Blocked_Cleaner.user.js
// @downloadURL        https://github.com/personwritep/Authentic_Blocked_Cleaner/raw/main/Authentic_Blocked_Cleaner.user.js
// ==/UserScript==


let readers=[]; // ブロックしたユーザーIDデータ


if(location.hostname=='blog.ameba.jp'){
    setTimeout(()=>{
        main_a();
    }, 2000); }


function main_a(){
    let retry=0;
    let interval=setInterval(wait_target, 200);
    function wait_target(){
        retry++;
        if(retry>10){ // リトライ制限 10回 2secまで
            clearInterval(interval); }
        let target=document.querySelector('.BlogWebBlock_next-button__OfEW6 button');
        if(target){
            target.click(); }}


    let block_item=document.querySelectorAll('.BlogWebBlock_item__2YbpR');
    for(let k=0; k<block_item.length; k++){
        let href_row=block_item[k].querySelector('a').getAttribute('href');
        let id=href_row.split('/')[3];
        if(id){
            readers.push(id); }}

    disp_panel(0);
    file_act();
    close();

} // main_a()




if(location.hostname=='ameblo.jp'){
    setTimeout(()=>{
        main_b();
    }, 1000);
}


function main_b(){
    if(location.hostname=='ameblo.jp'){
        disp_panel(1);
        file_act();
        unsubscribe();
        close();
   }

} // main_b()




function disp_panel(n){

    let help_url='https://ameblo.jp/personwritep/entry-12962260963.html';

    let SVG_h=
        '<svg class="help_ABC" height="22" width="22"  viewBox="0 0 200 200">'+
        '<path d="M89 22C71 25 54 33 41 46C7 81 11 142 50 171C58 177 68 182 78 18'+
        '5C90 188 103 189 115 187C126 185 137 181 146 175C155 169 163 162 169 153'+
        'C190 123 189 80 166 52C147 30 118 18 89 22z" style="fill:#888;"></path>'+
        '<path d="M67 77C73 75 78 72 84 70C94 66 114 67 109 83C106 91 98 95 93 10'+
        '1C86 109 83 116 83 126L111 126C112 114 122 108 129 100C137 90 141 76 135'+
        ' 64C127 45 101 45 84 48C80 49 71 50 68 54C67 56 67 59 67 61L67 77M85 143'+
        'L85 166L110 166L110 143L85 143z" style="fill:#fff;"></path>'+
        '</svg>';


    let panel=
        '<div id="modal_ABC">'+
        '<div id="panel_ABC">'+
        '<div class="ABC1">'+
        '<a href="'+ help_url +'" target="_blank" rel="noopener noreferrer">'+
        SVG_h +'</a>';
    if(n==1){
        panel+=
        '<input class="import sw_abc" type="submit" value="Read Blocked ID Backup">'+
        '<input class="file_input" type="file">'+
        '<span class="data_disp">　</span>'+
        '<input class="check sw_abc" type="submit" value="Check">'; }
    if(n==0){
        panel+=
            '<input class="export sw_abc" type="submit" value="Blocked ID Backup">'; }
    panel+=
        '<input class="close sw_abc" type="submit" value="✖">'+
        '</div>';
    if(n==1){
        panel+=
        '<div class="ABC2">'+
        '<ul></ul></div>'; }
    panel+=
        '</div>'+
        '<style>'+
        'html { overflow: hidden; } '+
        '#modal_ABC { '+
        'position: fixed; top: 0; left: 0; z-index: 6000; width: 100%; height: 100%; } '+
        '#panel_ABC { position: absolute; top: 100px; right: 40px; '+
        'display: flex; flex-direction: column; width: auto; padding: 12px 15px 12px; '+
        'font: normal 16px/16px Meiryo; color: #666; background: #e0f0fd; '+
        'border: 1px solid #ccc; border-radius: 2px; box-shadow: 0 0 0 100vw #00000080; } '+
        '.sw_abc { padding: 2px 6px 0; height: 28px;  cursor: pointer; '+
        'border: 1px solid #999; border-radius: 2px; background: #f0f0f0; } '+
        '#panel_ABC .help_ABC { margin: 0 6px -5px 0; } '+
        '#panel_ABC .import { margin: 0 10px; } '+
        '#panel_ABC .file_input { display: none; } '+
        '#panel_ABC .data_disp { display: inline-block; width: 125px; height: 28px; '+
        'padding: 6px 6px 0; margin-right: 10px; box-sizing: border-box; vertical-align: -8px; '+
        'font: normal 16px/16px Meiryo; border: 1px solid #ccc; color: #000; background: #fff; '+
        'overflow-x: hidden; white-space: nowrap; text-overflow: ellipsis; } '+
        '#panel_ABC .check { margin: 0 20px; } '+
        '#panel_ABC .export { margin: 0 30px 0 10px; } '+

        '#panel_ABC .ABC2 { margin: 12px 0; height: calc(100vh - 300px); overflow-y: scroll; '+
        'font: normal 16px Meiryo; color: #000; background: #fff; } '+
        '#panel_ABC .ABC2 li { padding: 5px 12px 3px; border-bottom: 1px solid #ccc; } '+
        '#panel_ABC .dn { display: inline-block; min-width: 30px; font-size: 12px; text-align: left; } '+
        '#panel_ABC .d0 { display: inline-block; width: 300px; } '+
        '#panel_ABC .d1 { display: inline-block; width: 150px; } '+
        '#panel_ABC .d2 { display: inline-block; width: 150px; } '+
        '</style>'+
        '</div>';

    if(!document.querySelector('#panel_ABC')){
        document.body.insertAdjacentHTML('beforeend', panel); }

} // disp_panel()



function file_act(){
    let imp=document.querySelector('#panel_ABC .import');
    let file_input=document.querySelector('#panel_ABC .file_input');
    let exp=document.querySelector('#panel_ABC .export');

    if(imp && file_input){
        imp.onclick=function(event){
            file_input.click(); }

        file_input.addEventListener('change' , function(){
            if(!(file_input.value)) return; // ファイルが選択されない場合
            let file_list=file_input.files;
            if(!file_list) return; // ファイルリストが選択されない場合
            let file=file_list[0];
            if(!file) return; // ファイルが無い場合

            if(file.name.startsWith('ABC')){ // ファイル名の確認
                let file_reader=new FileReader();
                file_reader.readAsText(file);
                file_reader.onload=function(){

                    let data_in=JSON.parse(file_reader.result);
                    readers=data_in;
                    setTimeout(()=>{
                        let data_disp=document.querySelector('#panel_ABC .data_disp');
                        if(data_disp){
                            data_disp.textContent=file.name; } // ファイル名を表示
                    }, 200);

                    setTimeout(()=>{
                        disp_list();
                    }, 200);
                }
            }
            else{
                alert(
                    "❌　Authentic Blocked Cleaner の Exportファイルではありません\n"+
                    "　　 Importファイルは「ABC.json」の名前です"); }


            setTimeout(()=>{
                this.value=null; // 同ファイルの再読込みを可能にする
            }, 1000);
        });

    } // if(imp && file_input)



    if(exp){
        exp.onclick=function(){
                let write_json=JSON.stringify(readers); //「フォロワー履歴」を書出す
                let blob=new Blob([write_json], {type: 'application/json'});

                let a_elem=document.createElement('a');
                a_elem.href=URL.createObjectURL(blob);
                a_elem.download='ABC.json'; // 保存ファイル名
                a_elem.click();
                URL.revokeObjectURL(a_elem.href);
          }

    } // if(exp)

} // file_act()



function disp_list(){
    let ul=document.querySelector('#panel_ABC .ABC2 ul');
    let li='';
    if(ul){
        for(let k=0; k<readers.length; k++){
            li+=
                '<li>'+
                '<span class="dn">'+ (k/1+1) +'</span>'+
                '<span class="d0">'+ readers[k] +'</span>';
            li+='</li>';
        }

        if(ul.querySelectorAll('li')){
            ul.innerHTML=''; }
        ul.insertAdjacentHTML('beforeend', li );

    }
} // disp_list()



function check_li(){
    let li=document.querySelectorAll('#panel_ABC li');
    if(li.length>0){
        return true; }}



function unsubscribe(){
    let check=document.querySelector('#panel_ABC .check');
    if(check){
        check.onclick=function(){
            if(check_li()){
                let panel_li=document.querySelectorAll('#panel_ABC li');

                let count=0; // チェックしたIDのカウント
                let count_d=0; // 退会者のカウント
                for(let i=0; i<panel_li.length; i++){
                    let id=panel_li[i].querySelector('.d0').textContent;
                    count+=1;

                    if(check_id(id)){
                        panel_li[i].style.background='#2196f395';
                        count_d+=1; }
                    }

                alert(
                    '退会者を調査しました \n'+
                    '　　　▶ 調査した件数: '+ count +' 件\n'+
                    '　　　▶ 退会ブログの件数: '+ count_d +' 件' );

            }}

    } // if(check)


    function check_id(id){
        let url='https://ameblo.jp/'+ id;
        if(load(url)!=200){
            return true; } // target_urlが無い時に true

        function load(_url){
            let xhr;
            xhr=new XMLHttpRequest();
            xhr.open("HEAD", _url, false); // 同期モード
            xhr.send();
            return xhr.status; }}

} // unsubscribe()



function close(){
    let close=document.querySelector('#panel_ABC .close');
    if(close){
        close.onclick=function(){
            let panel=document.querySelector('#modal_ABC');
            if(panel){
                panel.remove(); }}}

} // close()
