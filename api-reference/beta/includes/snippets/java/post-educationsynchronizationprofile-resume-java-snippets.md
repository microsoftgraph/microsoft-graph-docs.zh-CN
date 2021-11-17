---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7bc466543e58f80740f8714831d530d0b4827d17535de5815bc4c8a0e83a60d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .resume()
    .buildRequest()
    .post();

```