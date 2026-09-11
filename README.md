# Timbrado L&O

Ferramenta interna do Condomínio Rural Lívio J. Andrighetti e Outro para
inserir cabeçalho, rodapé e número em contratos e aditivos, e gerar o nome
do arquivo no padrão da empresa.

Versão desta publicação: **11/09/2026**

## Como publicar (GitHub Pages)

Não precisa instalar nada nem usar linha de comando.

1. Em <https://github.com/new>, crie um repositório — por exemplo
   `timbrado-lo`. Pode deixar **Public**; se preferir **Private**, veja a
   observação no fim.
2. Na tela do repositório vazio, clique em **uploading an existing file**
   (ou, se o repositório já tiver arquivos, **Add file → Upload files**).
3. Arraste para lá **todos os arquivos desta pasta**, inclusive o
   `.nojekyll` (ele é importante: garante que o site seja servido
   exatamente como está). Clique em **Commit changes**.
4. Vá em **Settings → Pages**. Em *Build and deployment*, escolha
   **Deploy from a branch**, branch **main** e pasta **/ (root)**. Salve.
5. Em um ou dois minutos o endereço aparece nessa mesma tela:
   `https://SEU-USUARIO.github.io/timbrado-lo/`
   O guia dos usuários fica em `.../guia.pdf`.

### Pela linha de comando (alternativa)

```bash
git init -b main
git add .
git commit -m "Timbrado L&O"
git remote add origin https://github.com/SEU-USUARIO/timbrado-lo.git
git push -u origin main
```

Depois, o passo 4 acima (Settings → Pages) continua sendo necessário uma
única vez.

## Como atualizar depois

Substitua o `index.html` pelo novo (**Add file → Upload files**, ou
`git add index.html && git commit -m "atualiza" && git push`). O GitHub
republica sozinho em cerca de um minuto. A data da versão aparece no alto
da tela da ferramenta, o que facilita conferir se o que está no ar é o mais
recente.

## Observações

- **Nenhum contrato sai do computador de quem usa.** A página monta o PDF
  dentro do próprio navegador; o servidor só entrega o arquivo da
  ferramenta. Nada é enviado nem armazenado no GitHub.
- O histórico de documentos timbrados fica no navegador de cada pessoa.
- **O endereço do GitHub Pages é público**, mesmo que o repositório seja
  privado (site privado só existe em planos Enterprise). Quem tiver o link
  consegue abrir. Para não aparecer em buscas, a página já vem com a marcação
  `noindex` no próprio HTML — é ela que vale aqui. (O `robots.txt` incluído
  só tem efeito se um dia o site for para um domínio próprio ou para um
  endereço do tipo `usuario.github.io` na raiz; em `usuario.github.io/repo/`
  os buscadores não o consultam.) Como a ferramenta não guarda nenhum dado, o
  que fica exposto é apenas a logo e os dados de contato do rodapé — os
  mesmos que já aparecem nos contratos. Se isso não for aceitável, use a
  hospedagem própria (HostGator), onde dá para proteger a pasta com senha.
