---
title: objectMapping 资源类型
description: 定义给定对象如何从源目录同步到目标目录。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94aa85c198ea67a4c53fc5b56d342188835b0ace
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133178"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="3772b-103">objectMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="3772b-103">objectMapping resource type</span></span>

<span data-ttu-id="3772b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3772b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3772b-105">定义给定对象如何从源目录同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="3772b-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="3772b-106">具体而言，它定义源目录中的对象如何与目标目录中的对象匹配，使用 (（如果任何) 范围筛选器）决定我们是否要设置给定对象，以及对象属性如何从源目录转换到目标目录。</span><span class="sxs-lookup"><span data-stu-id="3772b-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="3772b-107">对象映射是同步规则的主要部分，并且[](synchronization-synchronizationrule.md)作为同步架构的一[部分进行更新](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="3772b-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3772b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3772b-108">Properties</span></span>

| <span data-ttu-id="3772b-109">属性</span><span class="sxs-lookup"><span data-stu-id="3772b-109">Property</span></span>      | <span data-ttu-id="3772b-110">类型</span><span class="sxs-lookup"><span data-stu-id="3772b-110">Type</span></span>      | <span data-ttu-id="3772b-111">说明</span><span class="sxs-lookup"><span data-stu-id="3772b-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="3772b-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="3772b-112">attributeMappings</span></span>  |<span data-ttu-id="3772b-113">[attributeMapping](synchronization-attributemapping.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3772b-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="3772b-114">属性映射定义从源对象映射到目标对象的属性及其流动方法。</span><span class="sxs-lookup"><span data-stu-id="3772b-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="3772b-115">许多函数都可用于支持原始源值的转换。</span><span class="sxs-lookup"><span data-stu-id="3772b-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="3772b-116">enabled</span><span class="sxs-lookup"><span data-stu-id="3772b-116">enabled</span></span>        |<span data-ttu-id="3772b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3772b-117">Boolean</span></span>    |<span data-ttu-id="3772b-118">When `true` ， this object mapping will be processed during synchronization.</span><span class="sxs-lookup"><span data-stu-id="3772b-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="3772b-119">When `false` ， this object mapping will be skipped.</span><span class="sxs-lookup"><span data-stu-id="3772b-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="3772b-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="3772b-120">flowTypes</span></span>      |<span data-ttu-id="3772b-121">objectFlowTypes</span><span class="sxs-lookup"><span data-stu-id="3772b-121">objectFlowTypes</span></span>    |<span data-ttu-id="3772b-122">为此对象映射启用了哪些流类型。</span><span class="sxs-lookup"><span data-stu-id="3772b-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="3772b-123">`Add` 在目标目录中创建新对象、修改现有对象和取消设置 `Update` `Delete` 现有用户。</span><span class="sxs-lookup"><span data-stu-id="3772b-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="3772b-124">默认值为 `Add, Update, Delete` 。</span><span class="sxs-lookup"><span data-stu-id="3772b-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="3772b-125">metadata</span><span class="sxs-lookup"><span data-stu-id="3772b-125">metadata</span></span>       |<span data-ttu-id="3772b-126">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="3772b-126">metadataEntry collection</span></span>    |<span data-ttu-id="3772b-127">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3772b-127">Additional extension properties.</span></span> <span data-ttu-id="3772b-128">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="3772b-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="3772b-129">name</span><span class="sxs-lookup"><span data-stu-id="3772b-129">name</span></span>           |<span data-ttu-id="3772b-130">字符串</span><span class="sxs-lookup"><span data-stu-id="3772b-130">String</span></span>     |<span data-ttu-id="3772b-131">对象映射的友好名称。</span><span class="sxs-lookup"><span data-stu-id="3772b-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="3772b-132">范围</span><span class="sxs-lookup"><span data-stu-id="3772b-132">scope</span></span>          |[<span data-ttu-id="3772b-133">filter</span><span class="sxs-lookup"><span data-stu-id="3772b-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="3772b-134">定义在决定是否应设置给定对象时使用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="3772b-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="3772b-135">例如，你可能希望仅预配位于美国的用户。</span><span class="sxs-lookup"><span data-stu-id="3772b-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="3772b-136">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="3772b-136">sourceObjectName</span></span>           |<span data-ttu-id="3772b-137">字符串</span><span class="sxs-lookup"><span data-stu-id="3772b-137">String</span></span>     |<span data-ttu-id="3772b-138">源目录中对象的名称。</span><span class="sxs-lookup"><span data-stu-id="3772b-138">Name of the object in the source directory.</span></span> <span data-ttu-id="3772b-139">必须与源目录定义中的 [对象名称匹配](synchronization-directorydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="3772b-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="3772b-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="3772b-140">targetObjectName</span></span>           |<span data-ttu-id="3772b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="3772b-141">String</span></span>     |<span data-ttu-id="3772b-142">目标目录中对象的名称。</span><span class="sxs-lookup"><span data-stu-id="3772b-142">Name of the object in target directory.</span></span> <span data-ttu-id="3772b-143">必须与目标目录定义中的 [对象名称匹配](synchronization-directorydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="3772b-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3772b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3772b-144">JSON representation</span></span>

<span data-ttu-id="3772b-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3772b-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
  "attributeMappings": [{"@odata.type": "microsoft.graph.attributeMapping"}],
  "enabled": true,
  "flowTypes": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String",
  "scope": {"@odata.type": "microsoft.graph.filter"},
  "sourceObjectName": "String",
  "targetObjectName": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="3772b-146">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="3772b-146">JSON Example</span></span>

<!-- {
  "blockType": "example",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
    "attributeMappings": [
        {
            "defaultValue": "True",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Not([IsSoftDeleted])",
                "name": "Not",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[IsSoftDeleted]",
                            "name": "IsSoftDeleted",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "IsActive"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Mid([userPrincipalName], 1, 8)",
                "name": "Mid",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[userPrincipalName]",
                            "name": "userPrincipalName",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "start",
                        "value": {
                            "expression": "\"1\"",
                            "name": "1",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "length",
                        "value": {
                            "expression": "\"8\"",
                            "name": "8",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "Alias"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[mail]",
                "name": "mail",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Email"
        },
        {
            "defaultValue": "ISO-8859-1",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "EmailEncodingKey"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "LanguageLocaleKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[givenName]",
                "name": "givenName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "FirstName"
        },
        {
            "defaultValue": ".",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[surname]",
                "name": "surname",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "LastName"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
                "name": "Replace",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[preferredLanguage]",
                            "name": "preferredLanguage",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "Find",
                        "value": {
                            "expression": "\"-\"",
                            "name": "-",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "Replacement",
                        "value": {
                            "expression": "\"_\"",
                            "name": "_",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "LocaleSidKey"
        },
        {
            "defaultValue": "Chatter Free User",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "SingleAppRoleAssignment([appRoleAssignments])",
                "name": "SingleAppRoleAssignment",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[appRoleAssignments]",
                            "name": "appRoleAssignments",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "ProfileName"
        },
        {
            "defaultValue": "America/Los_Angeles",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "TimeZoneSidKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 1,
            "source": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Username"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsCallCenterAutoLogin"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsMarketingUser"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsOfflineUser"
        }
    ],
    "enabled": true,
    "flowTypes": "Add, Update, Delete",
    "metadata": [
        {
            "key": "IsCustomerDefined",
            "value": "false"
        },
        {
            "key": "DisableMonitoringForChanges",
            "value": "false"
        },
        {
            "key": "Disposition",
            "value": "\"Normal\""
        },
        {
            "key": "ExcludeFromReporting",
            "value": "false"
        },
        {
            "key": "EscrowBehavior",
            "value": "\"Default\""
        },
        {
            "key": "Unsynchronized",
            "value": "false"
        }
    ],
    "name": "Synchronize Azure Active Directory Users to salesforce.com",
    "scope": null,
    "sourceObjectName": "User",
    "targetObjectName": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


