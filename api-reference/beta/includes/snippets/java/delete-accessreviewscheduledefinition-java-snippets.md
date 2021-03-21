---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aa89307e76ea047db4e63b9e2f985492761e335
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982777"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("29f2d16e-9ca6-4052-bbfe-802c48981fd8")
    .buildRequest()
    .delete();

```