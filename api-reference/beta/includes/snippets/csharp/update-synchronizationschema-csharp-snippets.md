---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aa41a0da7bd7dbc8804389da83abee627e29bce
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = new SynchronizationSchema
{
    Directories = (ISynchronizationSchemaDirectoriesCollectionPage)new List<DirectoryDefinition>()
    {
        new DirectoryDefinition
        {
            Name = "Azure Active Directory",
            Objects = new List<ObjectDefinition>()
            {
                new ObjectDefinition
                {
                    Name = "User",
                    Attributes = new List<AttributeDefinition>()
                    {
                        new AttributeDefinition
                        {
                            Name = "userPrincipalName",
                            Type = AttributeType.String
                        }
                    }
                }
            }
        },
        new DirectoryDefinition
        {
            Name = "Salesforce"
        }
    },
    SynchronizationRules = new List<SynchronizationRule>()
    {
        new SynchronizationRule
        {
            Name = "USER_TO_USER",
            SourceDirectoryName = "Azure Active Directory",
            TargetDirectoryName = "Salesforce",
            ObjectMappings = new List<ObjectMapping>()
            {
                new ObjectMapping
                {
                    SourceObjectName = "User",
                    TargetObjectName = "User",
                    AttributeMappings = new List<AttributeMapping>()
                    {
                        new AttributeMapping
                        {
                            Source = new AttributeMappingSource
                            {
                            },
                            TargetAttributeName = "userName"
                        }
                    }
                }
            }
        }
    }
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema
    .Request()
    .PutAsync(synchronizationSchema);

```