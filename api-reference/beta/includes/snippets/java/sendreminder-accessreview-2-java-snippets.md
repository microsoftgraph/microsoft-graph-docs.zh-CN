---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 793822b2009e9744e2b7a830e7cecc8612a86609
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943056"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("04e5c3b2-9db2-40d3-a204-128f4956ae8e").instances("70463350-742e-4909-bfa5-bc23447bd002")
    .sendReminder()
    .buildRequest()
    .post();

```