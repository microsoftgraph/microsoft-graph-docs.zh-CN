---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e04f6801baa4451dac6915411ca94ea57a61a60fd95736a21c77d7e8cc3aa12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164070"
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

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema
    .Request()
    .PutAsync(synchronizationSchema);

```