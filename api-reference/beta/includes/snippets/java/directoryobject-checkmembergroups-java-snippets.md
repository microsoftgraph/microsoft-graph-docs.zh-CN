---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3870e2e7d47512953e084482810559d3c85617a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862475"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("fee2c45b-915a-4a64-b130-f4eb9e75525e");
groupIdsList.add("4fe90ae7-065a-478b-9400-e0a0e1cbd540");

graphClient.me()
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```