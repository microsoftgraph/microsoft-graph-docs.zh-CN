---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbc078957eb55cbd480ccd96fdc94851e840d971499390ce9fb9ebf71111b89e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378574"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffReason timeOffReason = graphClient.teams("{teamId}").schedule().timeOffReasons("{timeOffReasonId}")
    .buildRequest()
    .get();

```