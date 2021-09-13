---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5025c6b3346232e5bcd263b36757bca69ab7137aca2e4f9c00c7bd9bf878c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332066"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolCollectionWithReferencesPage schools = graphClient.education().me().schools()
    .buildRequest()
    .get();

```