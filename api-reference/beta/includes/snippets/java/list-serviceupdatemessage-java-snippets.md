---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86f7de07745dba6eb4d0caf9dd1307650b99776eb4f904afc0f8b77080d8629c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162176"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceUpdateMessageCollectionPage messages = graphClient.admin().serviceAnnouncement().messages()
    .buildRequest()
    .get();

```