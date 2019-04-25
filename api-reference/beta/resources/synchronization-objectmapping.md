---
title: objectMapping 资源类型
description: 定义给定对象应如何从源目录同步到目标目录。 具体而言, 它定义源目录中的对象应与目标目录中的对象匹配的方式, 应使用什么 (如果有) 作用域筛选器确定是否要预配给定的对象, 以及应如何转换对象属性源到目标目录。
localization_priority: Normal
ms.openlocfilehash: 274d401c28abc25d904c259b00a673f3c0a53888
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581751"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="b19de-104">objectMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="b19de-104">objectMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b19de-105">定义给定对象应如何从源目录同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="b19de-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="b19de-106">具体而言, 它定义源目录中的对象应与目标目录中的对象匹配的方式, 应使用什么 (如果有) 作用域筛选器确定是否要预配给定的对象, 以及应如何转换对象属性源到目标目录。</span><span class="sxs-lookup"><span data-stu-id="b19de-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="b19de-107">对象映射是[同步规则](synchronization-synchronizationrule.md)的主要部分, 并作为[同步架构](synchronization-synchronizationschema.md)的一部分进行更新。</span><span class="sxs-lookup"><span data-stu-id="b19de-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b19de-108">属性</span><span class="sxs-lookup"><span data-stu-id="b19de-108">Properties</span></span>

| <span data-ttu-id="b19de-109">属性</span><span class="sxs-lookup"><span data-stu-id="b19de-109">Property</span></span>      | <span data-ttu-id="b19de-110">类型</span><span class="sxs-lookup"><span data-stu-id="b19de-110">Type</span></span>      | <span data-ttu-id="b19de-111">说明</span><span class="sxs-lookup"><span data-stu-id="b19de-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="b19de-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="b19de-112">attributeMappings</span></span>  |<span data-ttu-id="b19de-113">[attributeMapping](synchronization-attributemapping.md)集合</span><span class="sxs-lookup"><span data-stu-id="b19de-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="b19de-114">属性映射定义将哪些属性从源对象映射到目标对象以及它们的流动方式。</span><span class="sxs-lookup"><span data-stu-id="b19de-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="b19de-115">有许多函数可用于支持原始源值的转换。</span><span class="sxs-lookup"><span data-stu-id="b19de-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="b19de-116">enabled</span><span class="sxs-lookup"><span data-stu-id="b19de-116">enabled</span></span>        |<span data-ttu-id="b19de-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b19de-117">Boolean</span></span>    |<span data-ttu-id="b19de-118">在`true`此情况下, 将在同步过程中处理此对象映射。</span><span class="sxs-lookup"><span data-stu-id="b19de-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="b19de-119">何时`false`, 将跳过此对象映射。</span><span class="sxs-lookup"><span data-stu-id="b19de-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="b19de-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="b19de-120">flowTypes</span></span>      |<span data-ttu-id="b19de-121">objectFlowType</span><span class="sxs-lookup"><span data-stu-id="b19de-121">objectFlowType</span></span>    |<span data-ttu-id="b19de-122">为此对象映射启用了哪些流类型。</span><span class="sxs-lookup"><span data-stu-id="b19de-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="b19de-123">`Add`在目标目录中创建新的对象`Update` , 修改现有的对象`Delete` , 并 deprovisions 现有用户。</span><span class="sxs-lookup"><span data-stu-id="b19de-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="b19de-124">默认值为`Add, Update, Delete`。</span><span class="sxs-lookup"><span data-stu-id="b19de-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="b19de-125">metadata</span><span class="sxs-lookup"><span data-stu-id="b19de-125">metadata</span></span>       |<span data-ttu-id="b19de-126">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="b19de-126">metadataEntry collection</span></span>    |<span data-ttu-id="b19de-127">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b19de-127">Additional extension properties.</span></span> <span data-ttu-id="b19de-128">除非明确提到, 否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="b19de-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="b19de-129">name</span><span class="sxs-lookup"><span data-stu-id="b19de-129">name</span></span>           |<span data-ttu-id="b19de-130">String</span><span class="sxs-lookup"><span data-stu-id="b19de-130">String</span></span>     |<span data-ttu-id="b19de-131">对象映射的人友好名称。</span><span class="sxs-lookup"><span data-stu-id="b19de-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="b19de-132">范围</span><span class="sxs-lookup"><span data-stu-id="b19de-132">scope</span></span>          |[<span data-ttu-id="b19de-133">filter</span><span class="sxs-lookup"><span data-stu-id="b19de-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="b19de-134">定义在决定是否应设置给定对象时要使用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="b19de-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="b19de-135">例如, 您可能希望仅预配位于美国的用户。</span><span class="sxs-lookup"><span data-stu-id="b19de-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="b19de-136">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="b19de-136">sourceObjectName</span></span>           |<span data-ttu-id="b19de-137">String</span><span class="sxs-lookup"><span data-stu-id="b19de-137">String</span></span>     |<span data-ttu-id="b19de-138">源目录中的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="b19de-138">Name of the object in the source directory.</span></span> <span data-ttu-id="b19de-139">必须与源[目录定义](synchronization-directorydefinition.md)中的对象名称相匹配。</span><span class="sxs-lookup"><span data-stu-id="b19de-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="b19de-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="b19de-140">targetObjectName</span></span>           |<span data-ttu-id="b19de-141">String</span><span class="sxs-lookup"><span data-stu-id="b19de-141">String</span></span>     |<span data-ttu-id="b19de-142">目标目录中的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="b19de-142">Name of the object in target directory.</span></span> <span data-ttu-id="b19de-143">必须与目标[目录定义](synchronization-directorydefinition.md)中的对象名称相匹配。</span><span class="sxs-lookup"><span data-stu-id="b19de-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b19de-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b19de-144">JSON representation</span></span>

<span data-ttu-id="b19de-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b19de-145">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="b19de-146">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="b19de-146">JSON Example</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-objectmapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
