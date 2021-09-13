---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2042af0ceb4ac59059f58678b7bf3258c0ba00eb45b58b698308d692070a249a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277581"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("8564a649-4f67-4e09-88e7-55def6530e88").instances("1234a649-4f67-1234-88e7-55def6530e88")
    .resetDecisions()
    .buildRequest()
    .post();

```