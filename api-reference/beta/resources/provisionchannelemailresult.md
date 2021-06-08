---
title: provisionChannelEmailResult 资源类型
description: 表示频道电子邮件设置操作的结果。
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac32dd0db4877dc01a13536689d414b0dcc1175f
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813229"
---
# <a name="provisionchannelemailresult-resource-type"></a><span data-ttu-id="376dd-103">provisionChannelEmailResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="376dd-103">provisionChannelEmailResult resource type</span></span>

<span data-ttu-id="376dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="376dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376dd-105">表示为[频道设置](..\api\channel-provisionemail.md)[的电子邮件地址](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="376dd-105">Represents the email address [provisioned](..\api\channel-provisionemail.md) for a [channel](channel.md).</span></span>

## <a name="properties"></a><span data-ttu-id="376dd-106">属性</span><span class="sxs-lookup"><span data-stu-id="376dd-106">Properties</span></span>
| <span data-ttu-id="376dd-107">属性</span><span class="sxs-lookup"><span data-stu-id="376dd-107">Property</span></span> | <span data-ttu-id="376dd-108">类型</span><span class="sxs-lookup"><span data-stu-id="376dd-108">Type</span></span>   | <span data-ttu-id="376dd-109">说明</span><span class="sxs-lookup"><span data-stu-id="376dd-109">Description</span></span>                               |
| :------- | :----- | :---------------------------------------- |
| <span data-ttu-id="376dd-110">email</span><span class="sxs-lookup"><span data-stu-id="376dd-110">email</span></span>    | <span data-ttu-id="376dd-111">String</span><span class="sxs-lookup"><span data-stu-id="376dd-111">String</span></span> | <span data-ttu-id="376dd-112">表示已设置的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="376dd-112">Represents the provisioned email address.</span></span> |

## <a name="relationships"></a><span data-ttu-id="376dd-113">关系</span><span class="sxs-lookup"><span data-stu-id="376dd-113">Relationships</span></span>
<span data-ttu-id="376dd-114">无。</span><span class="sxs-lookup"><span data-stu-id="376dd-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="376dd-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="376dd-115">JSON representation</span></span>
<span data-ttu-id="376dd-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="376dd-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
  "email": "String"
}
```
