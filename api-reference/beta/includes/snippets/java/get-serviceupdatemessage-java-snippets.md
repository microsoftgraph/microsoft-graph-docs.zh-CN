---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6314f5d57722f780c1bf8c6d926fb7387321ac8ffd5ba569ffcc382fb118787
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903290"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceUpdateMessage serviceUpdateMessage = graphClient.admin().serviceAnnouncement().messages("MC172851")
    .buildRequest()
    .get();

```