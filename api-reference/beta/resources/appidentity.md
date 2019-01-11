---
title: appIdentity 资源类型
description: 指示执行操作或已更改的应用程序的标识。 包含应用程序 Id、 名称、 服务主体 ID 和名称。 由 directoryAudit API 调用此资源
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855781"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="bc79d-105">appIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc79d-105">appIdentity resource type</span></span>
<span data-ttu-id="bc79d-106">指示执行操作或已更改的应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="bc79d-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="bc79d-107">包含应用程序 Id、 名称、 服务主体 ID 和名称。</span><span class="sxs-lookup"><span data-stu-id="bc79d-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="bc79d-108">由[directoryAudit](../api/directoryaudit-get.md) API 调用此资源</span><span class="sxs-lookup"><span data-stu-id="bc79d-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="bc79d-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc79d-109">Properties</span></span>
| <span data-ttu-id="bc79d-110">属性</span><span class="sxs-lookup"><span data-stu-id="bc79d-110">Property</span></span>     | <span data-ttu-id="bc79d-111">类型</span><span class="sxs-lookup"><span data-stu-id="bc79d-111">Type</span></span>   |<span data-ttu-id="bc79d-112">Description</span><span class="sxs-lookup"><span data-stu-id="bc79d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc79d-113">appId</span><span class="sxs-lookup"><span data-stu-id="bc79d-113">appId</span></span>|<span data-ttu-id="bc79d-114">String</span><span class="sxs-lookup"><span data-stu-id="bc79d-114">String</span></span>|<span data-ttu-id="bc79d-115">引用代表 Azure Active Directory 中的应用程序 Id 的唯一 guid。</span><span class="sxs-lookup"><span data-stu-id="bc79d-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="bc79d-116">displayName</span><span class="sxs-lookup"><span data-stu-id="bc79d-116">displayName</span></span>|<span data-ttu-id="bc79d-117">字符串</span><span class="sxs-lookup"><span data-stu-id="bc79d-117">String</span></span>|<span data-ttu-id="bc79d-118">指 Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="bc79d-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="bc79d-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="bc79d-119">servicePrincipalId</span></span>|<span data-ttu-id="bc79d-120">字符串</span><span class="sxs-lookup"><span data-stu-id="bc79d-120">String</span></span>|<span data-ttu-id="bc79d-121">指示在 Azure Active Directory 中的服务主体 Id 对应的应用程序的唯一 guid 引用。</span><span class="sxs-lookup"><span data-stu-id="bc79d-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="bc79d-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc79d-122">servicePrincipalName</span></span>|<span data-ttu-id="bc79d-123">String</span><span class="sxs-lookup"><span data-stu-id="bc79d-123">String</span></span>|<span data-ttu-id="bc79d-124">指的是服务主体名称是租户中的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="bc79d-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc79d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc79d-125">JSON representation</span></span>

<span data-ttu-id="bc79d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc79d-126">Here is a JSON representation of the resource.</span></span>

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
