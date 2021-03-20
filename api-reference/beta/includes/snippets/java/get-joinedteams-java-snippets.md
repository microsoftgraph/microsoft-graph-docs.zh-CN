---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c765aea7e2faa776912ee099e0356bc140f51792
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976836"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamCollectionWithReferencesPage joinedTeams = graphClient.me().joinedTeams()
    .buildRequest()
    .get();

```