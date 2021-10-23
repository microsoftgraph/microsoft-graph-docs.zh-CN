---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f63c6ee6be8babd489b7ba2ed4ca345f457b33d
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560350"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubjectRightsRequest subjectRightsRequest = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .buildRequest()
    .get();

```