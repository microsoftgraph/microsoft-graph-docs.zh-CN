---
title: smsAuthenticationMethodConfiguration 资源类型
description: 代表"短信身份验证方法"策略。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5a5e62e17e5b2e1cbc96ed96a44a0c483db981d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761035"
---
# <a name="smsauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="ca445-103">smsAuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca445-103">smsAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="ca445-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca445-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca445-105">代表"短信身份验证方法"策略。</span><span class="sxs-lookup"><span data-stu-id="ca445-105">Represents a Text Message authentication methods policy.</span></span> <span data-ttu-id="ca445-106">身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="ca445-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="ca445-107">方法</span><span class="sxs-lookup"><span data-stu-id="ca445-107">Methods</span></span>
|<span data-ttu-id="ca445-108">方法</span><span class="sxs-lookup"><span data-stu-id="ca445-108">Method</span></span>|<span data-ttu-id="ca445-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca445-109">Return type</span></span>|<span data-ttu-id="ca445-110">说明</span><span class="sxs-lookup"><span data-stu-id="ca445-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca445-111">Get</span><span class="sxs-lookup"><span data-stu-id="ca445-111">Get</span></span>](../api/smsauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="ca445-112">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca445-112">smsAuthenticationMethodConfiguration</span></span>](../resources/smsauthenticationmethodconfiguration.md)|<span data-ttu-id="ca445-113">读取 smsAuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ca445-113">Read the properties and relationships of a smsAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ca445-114">更新</span><span class="sxs-lookup"><span data-stu-id="ca445-114">Update</span></span>](../api/smsauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="ca445-115">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca445-115">smsAuthenticationMethodConfiguration</span></span>](../resources/smsauthenticationmethodconfiguration.md)|<span data-ttu-id="ca445-116">更新 smsAuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ca445-116">Update the properties of a smsAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ca445-117">删除</span><span class="sxs-lookup"><span data-stu-id="ca445-117">Delete</span></span>](../api/smsauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="ca445-118">无</span><span class="sxs-lookup"><span data-stu-id="ca445-118">None</span></span>|<span data-ttu-id="ca445-119">将 smsAuthenticationMethodConfiguration 对象还原到其默认配置。</span><span class="sxs-lookup"><span data-stu-id="ca445-119">Reverts the smsAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca445-120">属性</span><span class="sxs-lookup"><span data-stu-id="ca445-120">Properties</span></span>
|<span data-ttu-id="ca445-121">属性</span><span class="sxs-lookup"><span data-stu-id="ca445-121">Property</span></span>|<span data-ttu-id="ca445-122">类型</span><span class="sxs-lookup"><span data-stu-id="ca445-122">Type</span></span>|<span data-ttu-id="ca445-123">说明</span><span class="sxs-lookup"><span data-stu-id="ca445-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca445-124">id</span><span class="sxs-lookup"><span data-stu-id="ca445-124">id</span></span>|<span data-ttu-id="ca445-125">String</span><span class="sxs-lookup"><span data-stu-id="ca445-125">String</span></span>|<span data-ttu-id="ca445-126">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="ca445-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="ca445-127">state</span><span class="sxs-lookup"><span data-stu-id="ca445-127">state</span></span>|<span data-ttu-id="ca445-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="ca445-128">authenticationMethodState</span></span>|<span data-ttu-id="ca445-129">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="ca445-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca445-130">关系</span><span class="sxs-lookup"><span data-stu-id="ca445-130">Relationships</span></span>
|<span data-ttu-id="ca445-131">关系</span><span class="sxs-lookup"><span data-stu-id="ca445-131">Relationship</span></span>|<span data-ttu-id="ca445-132">类型</span><span class="sxs-lookup"><span data-stu-id="ca445-132">Type</span></span>|<span data-ttu-id="ca445-133">说明</span><span class="sxs-lookup"><span data-stu-id="ca445-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca445-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="ca445-134">includeTargets</span></span>|<span data-ttu-id="ca445-135">[smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca445-135">[smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="ca445-136">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="ca445-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca445-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca445-137">JSON representation</span></span>
<span data-ttu-id="ca445-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca445-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

