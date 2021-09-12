---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bfb0ccd0d1e488adf8a511f90f1ce9a17aee903d328a30359b9507f9da29795
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378324"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage members = graphClient.education().classes("{class-id}").members()
    .buildRequest()
    .get();

```