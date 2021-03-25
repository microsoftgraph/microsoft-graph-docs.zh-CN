---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55e72442d6805f5936f89a1deabd8c5637755bed
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209934"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShiftChangeRequestCollectionPage openShiftChangeRequests = graphClient.teams("{id}").schedule().openShiftChangeRequests()
    .buildRequest()
    .get();

```