---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a23783c26aea9cff942e96aeef5c539f1b10e073422de244617fb65b93d09689
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902708"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .stop()
    .buildRequest()
    .post();

```