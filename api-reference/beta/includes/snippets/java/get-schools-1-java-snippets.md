---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b12d3dc0fe8709497f329a52b4cdcef9835300bee28b276286143242af6c7944
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolCollectionWithReferencesPage schools = graphClient.education().classes("11014").schools()
    .buildRequest()
    .get();

```