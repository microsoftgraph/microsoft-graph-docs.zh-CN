---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5df1d21b1718eb80c4f5fcb2c691955cab7cca2ef93289d08ac3f81b1c48a072
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903784"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicyCollectionPage groupLifecyclePolicies = graphClient.groupLifecyclePolicies()
    .buildRequest()
    .get();

```