---
title: authenticationMethodsRegistrationCampaignIncludeTarget 资源类型
description: 允许提示用户和用户组设置目标身份验证方法。
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04dc753dd1a574bbf0b30d29b4b80375e7ab9a2c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682878"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a><span data-ttu-id="ff21a-103">authenticationMethodsRegistrationCampaignIncludeTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff21a-103">authenticationMethodsRegistrationCampaignIncludeTarget resource type</span></span>

<span data-ttu-id="ff21a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff21a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff21a-105">表示面向身份验证方法注册活动的用户和组。</span><span class="sxs-lookup"><span data-stu-id="ff21a-105">Represents the users and groups that are targeted for authentication method registration campaigns.</span></span> <span data-ttu-id="ff21a-106">只有策略启用以设置身份验证方法的用户和组作为目标。</span><span class="sxs-lookup"><span data-stu-id="ff21a-106">Only users and groups that are enabled by the policy to set up the authentication method are targeted.</span></span>

## <a name="properties"></a><span data-ttu-id="ff21a-107">属性</span><span class="sxs-lookup"><span data-stu-id="ff21a-107">Properties</span></span>
|<span data-ttu-id="ff21a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff21a-108">Property</span></span>|<span data-ttu-id="ff21a-109">类型</span><span class="sxs-lookup"><span data-stu-id="ff21a-109">Type</span></span>|<span data-ttu-id="ff21a-110">说明</span><span class="sxs-lookup"><span data-stu-id="ff21a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff21a-111">id</span><span class="sxs-lookup"><span data-stu-id="ff21a-111">id</span></span>|<span data-ttu-id="ff21a-112">String</span><span class="sxs-lookup"><span data-stu-id="ff21a-112">String</span></span>|<span data-ttu-id="ff21a-113">Azure AD 用户或组的对象标识符。</span><span class="sxs-lookup"><span data-stu-id="ff21a-113">The object identifier of an Azure AD user or group.</span></span>|
|<span data-ttu-id="ff21a-114">targetedAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ff21a-114">targetedAuthenticationMethod</span></span>|<span data-ttu-id="ff21a-115">String</span><span class="sxs-lookup"><span data-stu-id="ff21a-115">String</span></span>|<span data-ttu-id="ff21a-116">提示用户注册的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ff21a-116">The authentication method that the user is prompted to register.</span></span> <span data-ttu-id="ff21a-117">值必须为 `microsoftAuthenticator` 。</span><span class="sxs-lookup"><span data-stu-id="ff21a-117">The value must be `microsoftAuthenticator`.</span></span>|
|<span data-ttu-id="ff21a-118">targetType</span><span class="sxs-lookup"><span data-stu-id="ff21a-118">targetType</span></span>|<span data-ttu-id="ff21a-119">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="ff21a-119">authenticationMethodTargetType</span></span>|<span data-ttu-id="ff21a-120">身份验证方法目标的类型。</span><span class="sxs-lookup"><span data-stu-id="ff21a-120">The type of the authentication method target.</span></span> <span data-ttu-id="ff21a-121">可取值为：`user`、`group`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ff21a-121">Possible values are: `user`, `group`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff21a-122">关系</span><span class="sxs-lookup"><span data-stu-id="ff21a-122">Relationships</span></span>
<span data-ttu-id="ff21a-123">无。</span><span class="sxs-lookup"><span data-stu-id="ff21a-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff21a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff21a-124">JSON representation</span></span>
<span data-ttu-id="ff21a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff21a-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "targetedAuthenticationMethod": "String"
}
```
