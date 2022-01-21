---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d6ff613d724668dc6699fd69ab509a2be2994f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106803"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").customQuestions("80b5ddda-1e3b-4c9d-abe2-d606cc075e2e")
    .buildRequest()
    .delete();

```