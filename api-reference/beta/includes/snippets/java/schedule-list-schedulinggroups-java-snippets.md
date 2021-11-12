---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0c2528fe51e8e66b02b8d2cdddde707a833693fd4c0c3e685abcb2d8f7fce7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104731"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchedulingGroupCollectionPage schedulingGroups = graphClient.teams("{teamId}").schedule().schedulingGroups()
    .buildRequest()
    .get();

```