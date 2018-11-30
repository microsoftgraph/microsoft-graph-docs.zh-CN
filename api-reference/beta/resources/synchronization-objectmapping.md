---
title: objectMapping 资源类型
description: 定义如何给定的对象应同步从源目录到目标目录。 具体而言，它定义源目录中的对象与目标目录中某个对象的匹配方式什么 （如果有） 范围筛选器应确定如果我们想要设置给定的对象，以及应对象属性如何转换从到目标目录源。
ms.openlocfilehash: 5ecf406c3dab2f8d6fdcecadda4d5ff7bbb4f4d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043411"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="01f03-104">objectMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="01f03-104">objectMapping resource type</span></span>

> <span data-ttu-id="01f03-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01f03-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01f03-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01f03-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01f03-107">定义如何给定的对象应同步从源目录到目标目录。</span><span class="sxs-lookup"><span data-stu-id="01f03-107">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="01f03-108">具体而言，它定义源目录中的对象与目标目录中某个对象的匹配方式什么 （如果有） 范围筛选器应确定如果我们想要设置给定的对象，以及应对象属性如何转换从到目标目录源。</span><span class="sxs-lookup"><span data-stu-id="01f03-108">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="01f03-109">对象映射主[同步规则](synchronization-synchronizationrule.md)属于和更新[同步架构](synchronization-synchronizationschema.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="01f03-109">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="01f03-110">属性</span><span class="sxs-lookup"><span data-stu-id="01f03-110">Properties</span></span>

| <span data-ttu-id="01f03-111">属性</span><span class="sxs-lookup"><span data-stu-id="01f03-111">Property</span></span>      | <span data-ttu-id="01f03-112">类型</span><span class="sxs-lookup"><span data-stu-id="01f03-112">Type</span></span>      | <span data-ttu-id="01f03-113">说明</span><span class="sxs-lookup"><span data-stu-id="01f03-113">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="01f03-114">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="01f03-114">attributeMappings</span></span>  |<span data-ttu-id="01f03-115">[attributeMapping](synchronization-attributemapping.md)集合</span><span class="sxs-lookup"><span data-stu-id="01f03-115">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="01f03-116">属性映射定义从源对象映射到目标对象和如何应流哪些属性。</span><span class="sxs-lookup"><span data-stu-id="01f03-116">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="01f03-117">许多函数可供支持的原始源值转换。</span><span class="sxs-lookup"><span data-stu-id="01f03-117">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="01f03-118">enabled</span><span class="sxs-lookup"><span data-stu-id="01f03-118">enabled</span></span>        |<span data-ttu-id="01f03-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="01f03-119">Boolean</span></span>    |<span data-ttu-id="01f03-120">当`true`，将同步过程中处理此对象映射。</span><span class="sxs-lookup"><span data-stu-id="01f03-120">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="01f03-121">当`false`，将跳过此对象映射。</span><span class="sxs-lookup"><span data-stu-id="01f03-121">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="01f03-122">flowTypes</span><span class="sxs-lookup"><span data-stu-id="01f03-122">flowTypes</span></span>      |<span data-ttu-id="01f03-123">objectFlowType</span><span class="sxs-lookup"><span data-stu-id="01f03-123">objectFlowType</span></span>    |<span data-ttu-id="01f03-124">此对象映射为启用了哪些流类型。</span><span class="sxs-lookup"><span data-stu-id="01f03-124">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="01f03-125">`Add`在目标目录中，创建新对象`Update`修改现有对象和`Delete`取消设置现有用户。</span><span class="sxs-lookup"><span data-stu-id="01f03-125">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="01f03-126">默认值是`Add, Update, Delete`。</span><span class="sxs-lookup"><span data-stu-id="01f03-126">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="01f03-127">元数据</span><span class="sxs-lookup"><span data-stu-id="01f03-127">metadata</span></span>       |<span data-ttu-id="01f03-128">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="01f03-128">metadataEntry collection</span></span>    |<span data-ttu-id="01f03-129">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="01f03-129">Additional extension properties.</span></span> <span data-ttu-id="01f03-130">除非明确提到，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="01f03-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="01f03-131">name</span><span class="sxs-lookup"><span data-stu-id="01f03-131">name</span></span>           |<span data-ttu-id="01f03-132">字符串</span><span class="sxs-lookup"><span data-stu-id="01f03-132">String</span></span>     |<span data-ttu-id="01f03-133">对象映射的 human 友好名称。</span><span class="sxs-lookup"><span data-stu-id="01f03-133">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="01f03-134">scope</span><span class="sxs-lookup"><span data-stu-id="01f03-134">scope</span></span>          |[<span data-ttu-id="01f03-135">filter</span><span class="sxs-lookup"><span data-stu-id="01f03-135">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="01f03-136">定义一个筛选器，用于确定是否应设置给定的对象。</span><span class="sxs-lookup"><span data-stu-id="01f03-136">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="01f03-137">例如，您可能希望向只位于美国的设置用户。</span><span class="sxs-lookup"><span data-stu-id="01f03-137">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="01f03-138">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="01f03-138">sourceObjectName</span></span>           |<span data-ttu-id="01f03-139">字符串</span><span class="sxs-lookup"><span data-stu-id="01f03-139">String</span></span>     |<span data-ttu-id="01f03-140">源目录中对象的名称。</span><span class="sxs-lookup"><span data-stu-id="01f03-140">Name of the object in the source directory.</span></span> <span data-ttu-id="01f03-141">必须匹配源[目录定义](synchronization-directorydefinition.md)的对象名称。</span><span class="sxs-lookup"><span data-stu-id="01f03-141">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="01f03-142">目标</span><span class="sxs-lookup"><span data-stu-id="01f03-142">targetObjectName</span></span>           |<span data-ttu-id="01f03-143">字符串</span><span class="sxs-lookup"><span data-stu-id="01f03-143">String</span></span>     |<span data-ttu-id="01f03-144">目标目录中的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="01f03-144">Name of the object in target directory.</span></span> <span data-ttu-id="01f03-145">必须匹配从目标[目录定义](synchronization-directorydefinition.md)的对象名称。</span><span class="sxs-lookup"><span data-stu-id="01f03-145">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01f03-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01f03-146">JSON representation</span></span>

<span data-ttu-id="01f03-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01f03-147">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="01f03-148">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="01f03-148">JSON Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
