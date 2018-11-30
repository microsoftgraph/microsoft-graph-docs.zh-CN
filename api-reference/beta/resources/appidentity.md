---
title: appIdentity 资源类型
description: 指示执行操作或已更改的应用程序的标识。 包含应用程序 Id、 名称、 服务主体 ID 和名称。 由 directoryAudit API 调用此资源
ms.openlocfilehash: 6fcbe8dbb1e17139111c5f1fa9e8681cd1b996a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045294"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="8150e-105">appIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="8150e-105">appIdentity resource type</span></span>
<span data-ttu-id="8150e-106">指示执行操作或已更改的应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="8150e-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="8150e-107">包含应用程序 Id、 名称、 服务主体 ID 和名称。</span><span class="sxs-lookup"><span data-stu-id="8150e-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="8150e-108">由[directoryAudit](../api/directoryaudit-get.md) API 调用此资源</span><span class="sxs-lookup"><span data-stu-id="8150e-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="8150e-109">属性</span><span class="sxs-lookup"><span data-stu-id="8150e-109">Properties</span></span>
| <span data-ttu-id="8150e-110">属性</span><span class="sxs-lookup"><span data-stu-id="8150e-110">Property</span></span>     | <span data-ttu-id="8150e-111">类型</span><span class="sxs-lookup"><span data-stu-id="8150e-111">Type</span></span>   |<span data-ttu-id="8150e-112">说明</span><span class="sxs-lookup"><span data-stu-id="8150e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8150e-113">appId</span><span class="sxs-lookup"><span data-stu-id="8150e-113">appId</span></span>|<span data-ttu-id="8150e-114">String</span><span class="sxs-lookup"><span data-stu-id="8150e-114">String</span></span>|<span data-ttu-id="8150e-115">引用代表 Azure Active Directory 中的应用程序 Id 的唯一 guid。</span><span class="sxs-lookup"><span data-stu-id="8150e-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="8150e-116">displayName</span><span class="sxs-lookup"><span data-stu-id="8150e-116">displayName</span></span>|<span data-ttu-id="8150e-117">字符串</span><span class="sxs-lookup"><span data-stu-id="8150e-117">String</span></span>|<span data-ttu-id="8150e-118">指 Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="8150e-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="8150e-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="8150e-119">servicePrincipalId</span></span>|<span data-ttu-id="8150e-120">字符串</span><span class="sxs-lookup"><span data-stu-id="8150e-120">String</span></span>|<span data-ttu-id="8150e-121">指示在 Azure Active Directory 中的服务主体 Id 对应的应用程序的唯一 guid 引用。</span><span class="sxs-lookup"><span data-stu-id="8150e-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="8150e-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="8150e-122">servicePrincipalName</span></span>|<span data-ttu-id="8150e-123">String</span><span class="sxs-lookup"><span data-stu-id="8150e-123">String</span></span>|<span data-ttu-id="8150e-124">指的是服务主体名称是租户中的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="8150e-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8150e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8150e-125">JSON representation</span></span>

<span data-ttu-id="8150e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8150e-126">Here is a JSON representation of the resource.</span></span>

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