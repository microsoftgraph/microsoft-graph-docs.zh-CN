---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad43d1d0240da350d53bf4c485c069b2cd2bc8847ff6c2cc60e298e84250b655
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219376"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignmentCategories("96821157-5efb-4706-8ca2-a90b26c44852")
    .buildRequest()
    .get();

```