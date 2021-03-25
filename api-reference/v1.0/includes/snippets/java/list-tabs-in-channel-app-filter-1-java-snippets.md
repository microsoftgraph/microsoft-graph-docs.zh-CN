---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ada80280dbc9371e42cb1a148202e93896f7e5b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTabCollectionPage tabs = graphClient.teams("6903fa93-605b-43ef-920e-77c4729f8258").channels("19:33b76eea88574bd1969dca37e2b7a819@thread.skype").tabs()
    .buildRequest()
    .expand("teamsApp")
    .get();

```