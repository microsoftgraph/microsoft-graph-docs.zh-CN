---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 517ca7495d78353ed70eb0b6a4f2175f93eb4fdb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475988"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = new SynchronizationSchema
{
    Directories = new List<DirectoryDefinition>()
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