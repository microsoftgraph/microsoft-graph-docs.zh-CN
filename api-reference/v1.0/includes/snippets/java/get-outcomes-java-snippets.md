---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31476ffc669889259bb708f6964504950577e3411b1941fbffced51e0bbd9992
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279674"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationOutcomeCollectionPage outcomes = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").submissions("d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7").outcomes()
    .buildRequest()
    .get();

```