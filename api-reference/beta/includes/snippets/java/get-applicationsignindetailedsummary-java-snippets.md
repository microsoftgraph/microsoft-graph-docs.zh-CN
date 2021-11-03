---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccdba037c319eed0fcbec4fb298bf05fe7afb2829d8a27a7c2dbde9c3cdc7b98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104546"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationSignInDetailedSummary applicationSignInDetailedSummary = graphClient.reports().applicationSignInDetailedSummary("{id}")
    .buildRequest()
    .get();

```