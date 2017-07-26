<span data-ttu-id="7544a-p103">可以向其分配服务计划的对象。可能的值：</span><span class="sxs-lookup"><span data-stu-id="7544a-p103">The object the service plan can be assigned to. Possible values:</span></span>|可以向其分配服务计划的对象。可能的值：<br/><span data-ttu-id="7544a-127">“User” - 服务计划可分配给各个用户。</span><span class="sxs-lookup"><span data-stu-id="7544a-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="7544a-128">“Company” - 服务计划可分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="7544a-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7544a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7544a-129">JSON representation</span></span>

<span data-ttu-id="7544a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7544a-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
