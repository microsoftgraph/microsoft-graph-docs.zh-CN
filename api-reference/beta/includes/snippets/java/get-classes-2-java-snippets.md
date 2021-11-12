---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76a19e0da4756701caaf3a238094335060e9743047aa89a4fb1dff8ca0174585
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332302"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage classes = graphClient.education().schools("10002").classes()
    .buildRequest()
    .get();

```