---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43ee7bd009608c3a61d6d5c20721092fc72d7a037ca99c802308f077893004dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryCollectionPage assignmentCategories = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignmentCategories()
    .buildRequest()
    .get();

```