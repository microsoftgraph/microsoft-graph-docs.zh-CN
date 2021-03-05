---
title: applicationServicePrincipal 资源类型
description: 应用程序和 servicePrincipal 的组合。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 35abee6b3028111ce4237828b58492a546ff5d4b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476424"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="3b598-103">applicationServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b598-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="3b598-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b598-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b598-105">添加 Azure AD 应用程序库中的应用程序实例时，在目录中创建应用程序和[](../resources/application.md) [servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b598-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="3b598-106">**applicationServicePrincipal** 表示应用程序和 **servicePrincipal** 对象的连接。 </span><span class="sxs-lookup"><span data-stu-id="3b598-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="3b598-107">Methods</span><span class="sxs-lookup"><span data-stu-id="3b598-107">Methods</span></span>

<span data-ttu-id="3b598-108">无</span><span class="sxs-lookup"><span data-stu-id="3b598-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="3b598-109">属性</span><span class="sxs-lookup"><span data-stu-id="3b598-109">Properties</span></span>

| <span data-ttu-id="3b598-110">属性</span><span class="sxs-lookup"><span data-stu-id="3b598-110">Property</span></span>         | <span data-ttu-id="3b598-111">类型</span><span class="sxs-lookup"><span data-stu-id="3b598-111">Type</span></span>                                                 | <span data-ttu-id="3b598-112">说明</span><span class="sxs-lookup"><span data-stu-id="3b598-112">Description</span></span>                                                     |
| :--------------- | :--------------------------------------------------- | :-------------------------------------------------------------- |
| <span data-ttu-id="3b598-113">application</span><span class="sxs-lookup"><span data-stu-id="3b598-113">application</span></span>      | [<span data-ttu-id="3b598-114">application</span><span class="sxs-lookup"><span data-stu-id="3b598-114">application</span></span>](../resources/application.md)           | <span data-ttu-id="3b598-115">表示在 Azure Active Directory 中注册的应用程序。</span><span class="sxs-lookup"><span data-stu-id="3b598-115">Represents an application registered in Azure Active Directory.</span></span> |
| <span data-ttu-id="3b598-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="3b598-116">servicePrincipal</span></span> | [<span data-ttu-id="3b598-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="3b598-117">servicePrincipal</span></span>](../resources/serviceprincipal.md) | <span data-ttu-id="3b598-118">表示目录中的一个应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="3b598-118">Represents an instance of an application in a directory.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="3b598-119">关系</span><span class="sxs-lookup"><span data-stu-id="3b598-119">Relationships</span></span>

<span data-ttu-id="3b598-120">无</span><span class="sxs-lookup"><span data-stu-id="3b598-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b598-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b598-121">JSON representation</span></span>

<span data-ttu-id="3b598-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b598-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "keyProperty": "id"
}-->

```json
{
  "servicePrincipal": { "@odata.type": "microsoft.graph.servicePrincipal" },
  "application": { "@odata.type": "microsoft.graph.application" }
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
