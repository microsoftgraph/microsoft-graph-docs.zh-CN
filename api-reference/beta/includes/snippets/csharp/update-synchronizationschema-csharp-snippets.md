---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85f632dc112012f5d06f63f632a874d0b0ee584c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = new SynchronizationSchema
{
    Directories = new SynchronizationSchemaDirectoriesCollectionPage()
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