---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de5a27a289773683079cf570b39c35e295991d9a79a4f5fe0be32b83cebe630d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831182"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = graphClient.teams("893075dd-2487-4122-925f-022c42e20265")
    .buildRequest()
    .get();

```