---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ae6138e87e924e7c140020da85acddd76ee222f2b560bfd0ca36fd01724fd2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902739"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .applyDecisions()
    .buildRequest()
    .post();

```