---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fad63542a00a5d058a628917cced5e7d1630ebccc4933b5b8651d84f0ea8a6c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274074"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResourceCollectionPage resources = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").submissions("d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7").resources()
    .buildRequest()
    .get();

```