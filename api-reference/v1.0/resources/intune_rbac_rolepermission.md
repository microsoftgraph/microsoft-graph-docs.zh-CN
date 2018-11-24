# <a name="rolepermission-resource-type"></a><span data-ttu-id="392c6-101">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="392c6-101">rolePermission resource type</span></span>

> <span data-ttu-id="392c6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="392c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="392c6-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="392c6-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="392c6-104">属性</span><span class="sxs-lookup"><span data-stu-id="392c6-104">Properties</span></span>
|<span data-ttu-id="392c6-105">属性</span><span class="sxs-lookup"><span data-stu-id="392c6-105">Property</span></span>|<span data-ttu-id="392c6-106">类型</span><span class="sxs-lookup"><span data-stu-id="392c6-106">Type</span></span>|<span data-ttu-id="392c6-107">说明</span><span class="sxs-lookup"><span data-stu-id="392c6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="392c6-108">resourceActions</span><span class="sxs-lookup"><span data-stu-id="392c6-108">resourceActions</span></span>|<span data-ttu-id="392c6-109">[resourceAction](../resources/intune_rbac_resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="392c6-109">[resourceAction](../resources/intune_rbac_resourceaction.md) collection</span></span>|<span data-ttu-id="392c6-110">操作</span><span class="sxs-lookup"><span data-stu-id="392c6-110">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="392c6-111">关系</span><span class="sxs-lookup"><span data-stu-id="392c6-111">Relationships</span></span>
<span data-ttu-id="392c6-112">无</span><span class="sxs-lookup"><span data-stu-id="392c6-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="392c6-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="392c6-113">JSON Representation</span></span>
<span data-ttu-id="392c6-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="392c6-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```



