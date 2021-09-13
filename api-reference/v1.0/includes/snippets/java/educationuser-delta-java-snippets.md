---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d50885532e3e8828c803eb0e58e1928f5364303547a770c21b0968bcbb85cd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104982"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserDeltaCollectionPage delta = graphClient.education().users()
    .delta()
    .buildRequest()
    .get();

```