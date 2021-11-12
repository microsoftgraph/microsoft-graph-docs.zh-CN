---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87cf69dd69011415a8b0327c3abcf60ef0e284cec4c02ba9cd8edbc5bae305b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274390"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionPage classes = graphClient.education().classes()
    .buildRequest()
    .get();

```