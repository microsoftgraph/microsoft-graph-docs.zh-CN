---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cc1cd48f300d3ba922c4f682941f7f9b794b9a1561ca31413fd93cf67c2d471
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] stream = Base64.getDecoder().decode("The contents of the file goes here.");
    graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .put(stream);

```