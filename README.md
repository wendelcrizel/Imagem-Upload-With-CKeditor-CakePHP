Imagem-Upload-With-CKeditor-CakePHP
===================================

Sistema de upload com integração direta no form ou via ckeditor

INSTALAÇÃO
===================================

Clone ou desconpacte no diretório plugin do seu CakePHP

em app/Config/boostrap.php adicione:

CakePlugin::load('Imgadmin',array('routes'=>true));

ou

CakePlugin::loadAll(array('Imgadmin' => array('routes' => true)));

No seu form, ou layout, ou tema... bem, na sua view adicione os javascripts:

echo $this->Html->script(array('//ajax.googleapis.com/ajax/libs/jquery/2.0.0/jquery.min.js','imgadmin/admin.js','/imgadmin/js/ckeditor/ckeditor.js'));

Pronto, está tudo configurado

Usando
===================================

Para usar é fácil, apenas coloque um field hidden com class img-select, ex:

echo $this->Form->hidden('minhaimagem',array('class'=>'img-select'));

E para usar o ckeditor adicione a class ckeditor em um textarea

echo $this->Form->textarea('texto',array('class'=>'ckeditor'));

O CKeditor funciona normalmente, ou seja, com todas as funções e configurações que você precisar...

Bom uso!!!

Att. Erik Figueiredo
www.erikfigueiredo.com.br
