---
title: appIdentity 资源类型
description: 指示执行了操作或已更改的应用程序的标识。 包括应用程序 Id、名称、服务主体 ID 和名称。 此资源由 directoryAudit API 调用
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1878aa01f2a6594f102647b6642eab6f301fa91
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988595"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="93064-105">appIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="93064-105">appIdentity resource type</span></span>

<span data-ttu-id="93064-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93064-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93064-107">指示执行了操作或已更改的应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="93064-107">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="93064-108">包括应用程序 ID、名称和服务主体 ID 和名称。</span><span class="sxs-lookup"><span data-stu-id="93064-108">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="93064-109">[Get directoryAudit](../api/directoryaudit-get.md)操作使用此资源。</span><span class="sxs-lookup"><span data-stu-id="93064-109">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="93064-110">属性</span><span class="sxs-lookup"><span data-stu-id="93064-110">Properties</span></span>

| <span data-ttu-id="93064-111">属性</span><span class="sxs-lookup"><span data-stu-id="93064-111">Property</span></span>     | <span data-ttu-id="93064-112">类型</span><span class="sxs-lookup"><span data-stu-id="93064-112">Type</span></span>   |<span data-ttu-id="93064-113">说明</span><span class="sxs-lookup"><span data-stu-id="93064-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93064-114">appId</span><span class="sxs-lookup"><span data-stu-id="93064-114">appId</span></span>|<span data-ttu-id="93064-115">String</span><span class="sxs-lookup"><span data-stu-id="93064-115">String</span></span>|<span data-ttu-id="93064-116">表示唯一 GUID（表示 Azure Active Directory 中的应用程序 ID）。</span><span class="sxs-lookup"><span data-stu-id="93064-116">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="93064-117">displayName</span><span class="sxs-lookup"><span data-stu-id="93064-117">displayName</span></span>|<span data-ttu-id="93064-118">String</span><span class="sxs-lookup"><span data-stu-id="93064-118">String</span></span>|<span data-ttu-id="93064-119">引用 Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="93064-119">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="93064-120">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="93064-120">servicePrincipalId</span></span>|<span data-ttu-id="93064-121">String</span><span class="sxs-lookup"><span data-stu-id="93064-121">String</span></span>|<span data-ttu-id="93064-122">指在 Azure Active Directory 中指示对应应用程序的服务主体 Id 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="93064-122">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="93064-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="93064-123">servicePrincipalName</span></span>|<span data-ttu-id="93064-124">String</span><span class="sxs-lookup"><span data-stu-id="93064-124">String</span></span>|<span data-ttu-id="93064-125">引用服务主体名称是租户中的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="93064-125">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93064-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93064-126">JSON representation</span></span>

<span data-ttu-id="93064-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93064-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

