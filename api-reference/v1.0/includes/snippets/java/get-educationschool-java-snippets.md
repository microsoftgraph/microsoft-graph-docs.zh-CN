---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a64371e12b310e7e9a8a7594d23091157766ce03e2e4bbc1bc10bcd04adbceb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333969"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("{educationSchoolId}")
    .buildRequest()
    .get();

```