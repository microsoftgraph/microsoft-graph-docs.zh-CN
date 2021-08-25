---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7200a2aeb873b1a5ae9c6d72203955e9f1c5672e
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514458"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResource educationSubmissionResource = new EducationSubmissionResource();
EducationWordResource resource = new EducationWordResource();
resource.displayName = "Report.docx";
resource.fileUrl = "https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2";
educationSubmissionResource.resource = resource;

graphClient.education().classes("f4a941ff-9da6-4707-ba5b-0eae93cad0b4").assignments("3c77de7f-539b-49e1-9c96-1274f2f0ee3b").submissions("4af73d2b-6b9c-493f-0688-979087bed39b").resources()
    .buildRequest()
    .post(educationSubmissionResource);

```