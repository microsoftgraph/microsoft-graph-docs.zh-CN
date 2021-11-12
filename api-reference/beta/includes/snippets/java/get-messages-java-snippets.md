---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bdd5edae4245775d21d38facb8a07ecf4b9bf699f34a24aa38af8938bc84561
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105486"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .select("sender,subject")
    .get();

```