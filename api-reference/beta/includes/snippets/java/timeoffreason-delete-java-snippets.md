---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43cd8eaf5205d6756333dff8a8be88391ab7131a842869515eef746887f89d7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104669"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().timeOffReasons("{timeOffReasonId}")
    .buildRequest()
    .delete();

```