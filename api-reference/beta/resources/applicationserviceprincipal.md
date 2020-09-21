---
title: applicationServicePrincipal 资源类型
description: 应用程序和 servicePrincipal 的组合。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b45da6cd8533d9522d42428f6e222a669f17e681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050267"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="98d1e-103">applicationServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="98d1e-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="98d1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d1e-105">当添加了 Azure AD 应用程序库中的应用程序实例时，将在目录中创建 [application](../resources/application.md) 和 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98d1e-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="98d1e-106">**ApplicationServicePrincipal**表示**应用程序**和**servicePrincipal**对象的串联。</span><span class="sxs-lookup"><span data-stu-id="98d1e-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="98d1e-107">方法</span><span class="sxs-lookup"><span data-stu-id="98d1e-107">Methods</span></span>

<span data-ttu-id="98d1e-108">无</span><span class="sxs-lookup"><span data-stu-id="98d1e-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="98d1e-109">属性</span><span class="sxs-lookup"><span data-stu-id="98d1e-109">Properties</span></span>

| <span data-ttu-id="98d1e-110">属性</span><span class="sxs-lookup"><span data-stu-id="98d1e-110">Property</span></span> | <span data-ttu-id="98d1e-111">类型</span><span class="sxs-lookup"><span data-stu-id="98d1e-111">Type</span></span>        | <span data-ttu-id="98d1e-112">说明</span><span class="sxs-lookup"><span data-stu-id="98d1e-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98d1e-113">application</span><span class="sxs-lookup"><span data-stu-id="98d1e-113">application</span></span>|[<span data-ttu-id="98d1e-114">application</span><span class="sxs-lookup"><span data-stu-id="98d1e-114">application</span></span>](../resources/application.md)|<span data-ttu-id="98d1e-115">表示在 Azure Active Directory 中注册的应用程序。</span><span class="sxs-lookup"><span data-stu-id="98d1e-115">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="98d1e-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="98d1e-116">servicePrincipal</span></span>|[<span data-ttu-id="98d1e-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="98d1e-117">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="98d1e-118">表示目录中的一个应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="98d1e-118">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98d1e-119">关系</span><span class="sxs-lookup"><span data-stu-id="98d1e-119">Relationships</span></span>

<span data-ttu-id="98d1e-120">无</span><span class="sxs-lookup"><span data-stu-id="98d1e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98d1e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98d1e-121">JSON representation</span></span>

<span data-ttu-id="98d1e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98d1e-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


