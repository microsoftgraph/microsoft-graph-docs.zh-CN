---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18c3ead939416947b8966143f7b96c7c655f7f7f9b07e999915f8affccffc582
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104999"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments()
    .buildRequest()
    .get();

```