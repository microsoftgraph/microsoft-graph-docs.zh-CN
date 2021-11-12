---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c57195423fcee7e32add6109077bbcacb83f8a425d7020dc6fa26a772bece53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328801"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolCollectionPage schools = graphClient.education().schools()
    .buildRequest()
    .get();

```