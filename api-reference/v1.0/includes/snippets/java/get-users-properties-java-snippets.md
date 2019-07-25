---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d0e56df3ee0bbb39c89be8fe56d3160165f9910
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882798"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionPage users = graphClient.users()
    .buildRequest()
    .select("displayName,givenName,postalCode")
    .get();

```