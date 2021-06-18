---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 354badb6d6f8ca63531937594c4e0f64f67bcf2a
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993408"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = new EducationResource
{
    AssignmentResourceUrl = "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
    Resource = new EducationWordResource
    {
        DisplayName = "Report.docx",
        CreatedDateTime = DateTimeOffset.Parse("2017-10-21T07:52:53.9863696Z"),
        CreatedBy = new IdentitySet
        {
            Application = null,
            Device = null,
            User = new Identity
            {
                Id = "63cc91d2-59c7-4732-9594-35b91a26b340",
                DisplayName = null
            }
        },
        LastModifiedDateTime = DateTimeOffset.Parse("2017-10-21T07:52:53.9863696Z"),
        LastModifiedBy = new IdentitySet
        {
            Application = null,
            Device = null,
            User = new Identity
            {
                Id = "63cc91d2-59c7-4732-9594-35b91a26b340",
                DisplayName = null
            }
        },
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources
    .Request()
    .AddAsync(educationSubmissionResource);

```