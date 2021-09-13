---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2db65dbb729ff0bbad251d12ebf914ff03bfadbf196196edc2b74de2d91d2c25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106817"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTab teamsTab = new TeamsTab();
teamsTab.displayName = "My Contoso Tab - updated again";

graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs("794f0e4e-4d10-4bb5-9079-3a465a629eff")
    .buildRequest()
    .patch(teamsTab);

```