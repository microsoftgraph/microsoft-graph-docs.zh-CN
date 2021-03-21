---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cef41d444c9aa3c672aee533483fda7a03f293e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976712"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicyCollectionPage groupLifecyclePolicies = graphClient.groups("{id}").groupLifecyclePolicies()
    .buildRequest()
    .get();

```