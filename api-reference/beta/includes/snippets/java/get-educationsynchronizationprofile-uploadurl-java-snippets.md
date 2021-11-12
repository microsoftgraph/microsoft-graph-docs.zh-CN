---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a66426b458b894c2523251250713d51d3ce39f1e4cbe42faef372b487320d21c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162245"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.education().synchronizationProfiles("{id}")
    .uploadUrl()
    .buildRequest()
    .get();

```