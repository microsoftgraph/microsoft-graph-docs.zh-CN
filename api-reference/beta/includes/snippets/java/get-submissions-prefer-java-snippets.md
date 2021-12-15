---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed4dbb360b924989d138473adc195ebcec2329bc
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525845"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "include-unknown-enum-members"));

EducationSubmissionCollectionPage submissions = graphClient.education().classes("59069eb2-2a09-4d90-bb19-2089cc69d613").assignments("80da1069-a635-4913-813f-d775a5470a8f").submissions()
    .buildRequest( requestOptions )
    .get();

```