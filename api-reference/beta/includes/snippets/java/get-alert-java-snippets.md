---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bac22c2bf4fdfe3d36880869d80cd6e89e398050d17537eaed3b5238b54b54b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902530"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Alert alert = graphClient.security().alerts("{id}")
    .buildRequest()
    .get();

```